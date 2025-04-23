# Chapter IV: Solution Software Design
## 4.1. Strategic-Level Domain-Driven Design
### 4.1.1. EventStorming

Llevamos a cabo nuestro proceso de Event Storming utilizando la herramienta MURAL, donde construimos todo el flujo del sistema. Iniciamos con la fase de **Exploración No Estructurada**, en la que intercambiamos ideas y discutimos libremente los eventos del dominio, guiándonos por las recomendaciones establecidas para esta etapa.

![alt text](../img/image.png)

#### 4.1.1.1 Candidate Context Discovery.

- 
#### 4.1.1.2 Domain Message Flows Modeling.



#### 4.1.1.3 Bounded Context Canvases. 


### 4.1.2. Context Mapping.

### 4.1.3. Software Architecture.

#### 4.1.3.1. Software Architecture System Landscape Diagram.

#### 4.1.3.2. Software Architecture Context Level Diagrams.

#### 4.1.3.2. Software Architecture Container Level Diagrams.

#### 4.1.3.3. Software Architecture Deployment Diagrams.


## 4.2. Tactical-Level Domain-Driven Design
-
### 4.2.1. Bounded Context: Subscription & Payment

#### 4.2.1.1. Domain Layer.
En el núcleo del dominio se han definido los siguientes Agregados, que representan los conceptos más importantes del Bounded Context de Suscripciones.




## `Aggregates` 


### `Subscription` 

Representa la suscripción de un sensor. 
#### Atributos principales:

| Atributo     | Tipo                | Descripción                                                 |
|--------------|---------------------|-------------------------------------------------------------|
| `id`         | `Int`               | Identificador único de la suscripción                       |
| `startDate`  | `Date`              | Fecha de inicio de la suscripción                           |
| `endDate`    | `Date`              | Fecha de fin de la suscripción                              |
| `status`     | `SubscriptionStatus`| Estado actual de la suscripción (`ACTIVE`, `EXPIRED`, etc.) |
| `sensorId`   | `Int`               | Identificador del sensor asociado                           |
| `residentId` | `Int`               | Identificador del residente asociado                        |

#### Constructores:

- Por parámetros individuales 
- A partir de `CreateSubscriptionCommand`
- A partir de `UpdateSubscriptionStatusCommand`
- A partir de `UpdateSubscriptionEndDateCommand`
---


### `Payment` 

Representa el pago de una suscripción. 
#### Atributos principales:

| Atributo         | Tipo              | Descripción                         |
|------------------|-------------------|-------------------------------------|
| `id`             | `Int`             | Identificador único del pago        |
| `subscriptionId` | `Int`             | Relación con la suscripción asociada|
| `amount`         | `Decimal`         | Monto del pago                      |
| `status`         | `PaymentStatus`   | Estado del pago (PENDING, SUCCESS, etc.) |
| `method`         | `PaymentMethod`   | Método de pago (CARD, YAPE, etc.)   |
| `paidAt`         | `Date`            | Fecha en la que se realizó el pago  |    |

#### Constructores:

- Por parámetros individuales 
- A partir de `CreatePaymentCommand`
---

Los siguientes enumerados (enums) representan valores fijos que controlan el estado y comportamiento de las entidades del sistema dentro del contexto de suscripciones y pagos. Se utilizan para asegurar consistencia, facilitar validaciones y mejorar la legibilidad del código, evitando el uso de strings sueltos o valores mágicos.


### `SubscriptionStatus(Enum)` 

| Valor       | Descripción                                                  |
|-------------|--------------------------------------------------------------|
| ACTIVE      | La suscripción está activa y el sensor está en funcionamiento |
| EXPIRED     | La suscripción ha terminado su periodo de vigencia            |
| CANCELLED   | La suscripción fue cancelada antes de su vencimiento          |
| PENDING     | La suscripción ha sido creada pero aún no se ha activado      |

### `PaymentStatus (Enum)` 

 | Valor       | Descripción                                 |
|-------------|----------------------------------------------|
| PENDING     | El pago ha sido iniciado pero no completado  |
| SUCCESS     | El pago se procesó correctamente             |
| FAILED      | El intento de pago falló                     |
| CANCELLED   | El pago fue cancelado por el usuario o sistema |

### `PaymentMethod  (Enum)` 

| Valor         | Descripción                             |
|---------------|------------------------------------------|
| CARD          | Pago realizado con tarjeta               |
| YAPE          | Pago a través de la app Yape             |
| PLIN          | Pago a través de la app Plin             |
| BANK_TRANSFER | Transferencia bancaria                   |


## `Commands` 

### Subscription Commands

| Comando                         | Descripción                                                         |
|--------------------------------|----------------------------------------------------------------------|
| `CreateSubscriptionCommand`    | Crea una nueva suscripción, asignando un sensor a un residente con fechas definidas |
| `CancelSubscriptionCommand`    | Cancela una suscripción activa antes de su fecha de fin             |
| `UpdateSubscriptionEndDateCommand` | Modifica la fecha de finalización de la suscripción                 |
| `ExpireSubscriptionCommand`    | Marca una suscripción como expirada si ha superado su fecha de fin  |
| `ActivateSubscriptionCommand`  | Cambia el estado de una suscripción a `ACTIVE`                      |


### Payment Commands
| Comando                     | Descripción                                                       |
|----------------------------|--------------------------------------------------------------------|
| `CreatePaymentCommand`     | Registra un nuevo pago asociado a una suscripción                 |
| `UpdatePaymentStatusCommand` | Cambia el estado de un pago (`PENDING`, `SUCCESS`, `FAILED`, etc.) |


## `Queries` 


### Subscription Queries
| Query                                | Descripción                                                                      |
|-------------------------------------|----------------------------------------------------------------------------------|
| `GetSubscriptionByIdQuery`          | Obtiene una suscripción específica por su ID                                    |
| `GetSubscriptionsByResidentIdQuery`| Lista todas las suscripciones activas o históricas de un residente              |
| `GetActiveSubscriptionBySensorIdQuery` | Devuelve la suscripción activa de un sensor determinado                         |
| `GetAllActiveSubscriptionsQuery`    | Lista todas las suscripciones activas del sistema                               |


### Payment Queries
| Query                              | Descripción                                                    |
|-----------------------------------|----------------------------------------------------------------|
| `GetPaymentByIdQuery`             | Obtiene los detalles de un pago específico por su ID          |
| `GetPaymentsBySubscriptionIdQuery`| Lista todos los pagos hechos para una suscripción dada        |
| `GetRecentPaymentsByResidentIdQuery` | Devuelve los pagos recientes realizados por un residente      |

## `Repositories (Interfaces)` 
| Archivo                     | Descripción breve                                                                 |
|----------------------------|-------------------------------------------------------------------------------------|
| ISubscriptionRepository.cs | Define operaciones sobre suscripciones: `FindByIdAsync`, `FindByResidentIdAsync`, `FindActiveBySensorIdAsync`, `SaveAsync`, `UpdateStatusAsync` |
| IPaymentRepository.cs      | Define operaciones sobre pagos: `FindByIdAsync`, `FindBySubscriptionIdAsync`, `SaveAsync`, `UpdateStatusAsync`             |


## `Services` 
### Subscription

| Archivo                          | Descripción breve                                                                 |
|----------------------------------|-------------------------------------------------------------------------------------|
| ISubscriptionCommandService.cs  | Define comandos como crear, cancelar o renovar suscripciones.                     |
| ISubscriptionQueryService.cs    | Define consultas para obtener suscripciones (por residente, por sensor, por estado, por id). |

### Payment

| Archivo                      | Descripción breve                                                                 |
|------------------------------|-------------------------------------------------------------------------------------|
| IPaymentCommandService.cs   | Define comandos como registrar pago, actualizar estado o reintentar un pago.      |
| IPaymentQueryService.cs     | Define consultas para obtener pagos (por suscripción, por estado, por método, por id). |


#### 4.2.1.2. Interface Layer.

La carpeta `Interfaces/REST` expone los endpoints HTTP que permiten a clientes externos interactuar con la aplicación transformando solicitudes en comandos o queries y devolviendo respuestas.




## `Resources` 
Las clases `Resource` actúan como intermediarias que trasladan datos entre la API REST y la capa de aplicación.

| Archivo                           | Función                                                                 |
|----------------------------------|-------------------------------------------------------------------------|
| `CreateSubscriptionResource.cs`  | Recibe datos para registrar una nueva suscripción desde el cliente.    |
| `CancelSubscriptionResource.cs`  | Permite cancelar una suscripción existente.                            |
| `SubscriptionResource.cs`        | Devuelve información de una suscripción (GET).                         |
| `CreatePaymentResource.cs`       | Recibe datos para registrar un nuevo pago asociado a una suscripción.  |
| `PaymentResource.cs`             | Devuelve detalles del pago realizado (GET).                            |


## `Transform/Assemblers` 

Las clases ubicadas en la carpeta **Transform** (o también conocidas como **Assemblers**) se encargan de:

- Traducir los objetos **Resource** en **Command Objects** que serán procesados por la capa de aplicación.  
- Convertir las entidades del dominio en objetos **Resource** que se utilizarán para construir las respuestas de la API.

| Archivo                                             | Función                                                                 |
|-----------------------------------------------------|-------------------------------------------------------------------------|
| `CreateSubscriptionCommandFromResourceAssembler.cs` | Transforma `CreateSubscriptionResource` en `CreateSubscriptionCommand`. |
| `CreatePaymentCommandFromResourceAssembler.cs`      | Transforma `CreatePaymentResource` en `CreatePaymentCommand`.           |
| `SubscriptionResourceFromEntityAssembler.cs`        | Convierte una entidad `Subscription` en un `SubscriptionResource` limpio. |
| `PaymentResourceFromEntityAssembler.cs`             | Convierte una entidad `Payment` en un `PaymentResource` limpio.         |


## `Controllers` 
Cada entidad principal dentro del Bounded Context *Reservations* dispone de un **REST Controller**, encargado de exponer los endpoints públicos y coordinar la lógica de ejecución de la aplicación.

| Controlador              | Ruta base típica | Responsabilidad principal                                                                 |
|--------------------------|------------------|--------------------------------------------------------------------------------------------|
| `SubscriptionController.cs` | `/api/subscription` | Gestiona la creación, actualización y consulta de suscripciones.                          |
| `PaymentController.cs`      | `/api/payment`      | Maneja operaciones de pagos: registrar, consultar historial y actualizar estado de pago.  |

#### 4.2.1.3. Application Layer.

### Servicios de Aplicación – Gestión de Flujos de Negocio

## `CommandServices` 

## `QueryServices` 



#### 4.2.1.4. Infrastructure Layer.




#### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams.

#### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams.

##### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams.


##### 4.2.1.6.2. Bounded Context Database Design Diagram.


### 4.2.2. Bounded Context: BoundedContext
-
#### 4.2.2.1. Domain Layer.
-
#### 4.2.2.2. Interface Layer.
-
#### 4.2.2.3. Application Layer.
-
#### 4.2.2.4. Infrastructure Layer.
-
#### 4.2.2.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.2.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.2.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.2.6.2. Bounded Context Database Design Diagram.


### 4.2.3. Bounded Context: BoundedContext
-
#### 4.2.3.1. Domain Layer.
-
#### 4.2.3.2. Interface Layer.
-
#### 4.2.3.3. Application Layer.
-
#### 4.2.3.4. Infrastructure Layer.
-
#### 4.2.3.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.3.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.3.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.3.6.2. Bounded Context Database Design Diagram.


### 4.2.4. Bounded Context: BoundedContext
-
#### 4.2.4.1. Domain Layer.
-
#### 4.2.4.2. Interface Layer.
-
#### 4.2.4.3. Application Layer.
-
#### 4.2.4.4. Infrastructure Layer.
-
#### 4.2.4.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.4.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.4.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.4.6.2. Bounded Context Database Design Diagram.


### 4.2.5. Bounded Context: BoundedContext
-
#### 4.2.5.1. Domain Layer.
-
#### 4.2.5.2. Interface Layer.
-
#### 4.2.5.3. Application Layer.
-
#### 4.2.5.4. Infrastructure Layer.
-
#### 4.2.5.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.5.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.5.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.5.6.2. Bounded Context Database Design Diagram.


### 4.2.6. Bounded Context: BoundedContext
-
#### 4.2.6.1. Domain Layer.
-
#### 4.2.6.2. Interface Layer.
-
#### 4.2.6.3. Application Layer.
-
#### 4.2.6.4. Infrastructure Layer.
-
#### 4.2.6.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.6.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.6.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.6.6.2. Bounded Context Database Design Diagram.


### 4.2.7. Bounded Context: BoundedContext
-
#### 4.2.7.1. Domain Layer.
-
#### 4.2.7.2. Interface Layer.
-
#### 4.2.7.3. Application Layer.
-
#### 4.2.7.4. Infrastructure Layer.
-
#### 4.2.7.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.7.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.7.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.7.6.2. Bounded Context Database Design Diagram.


### 4.2.8. Bounded Context: BoundedContext
-
#### 4.2.8.1. Domain Layer.
-
#### 4.2.8.2. Interface Layer.
-
#### 4.2.8.3. Application Layer.
-
#### 4.2.8.4. Infrastructure Layer.
-
#### 4.2.8.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.8.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.8.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.8.6.2. Bounded Context Database Design Diagram.


### 4.2.9. Bounded Context: BoundedContext
-
#### 4.2.9.1. Domain Layer.
-
#### 4.2.9.2. Interface Layer.
-
#### 4.2.9.3. Application Layer.
-
#### 4.2.9.4. Infrastructure Layer.
-
#### 4.2.9.5. Bounded Context Software Architecture Component Level Diagrams.
-
#### 4.2.9.6. Bounded Context Software Architecture Code Level Diagrams.
-
##### 4.2.9.6.1. Bounded Context Domain Layer Class Diagrams.
-
##### 4.2.9.6.2. Bounded Context Database Design Diagram.
