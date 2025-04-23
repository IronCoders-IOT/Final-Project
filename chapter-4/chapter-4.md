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
### 4.2.1. Bounded Context: Subscription

#### 4.2.1.1. Domain Layer.

Dentro del dominio de Subscription, se encuentran las entidades y servicios esenciales para administrar las suscripciones y sus pagos asociados en la plataforma. Este dominio se encarga de gestionar el ciclo de vida completo de una suscripción, incluyendo su creación, activación, renovación, cancelación y expiración, así como el procesamiento y seguimiento de los pagos correspondientes. Las entidades clave, como Subscription y Payment, definen la estructura y comportamiento de las suscripciones (fechas, estado, sensores vinculados) y los pagos (métodos, montos y estados), mientras que los servicios de dominio garantizan operaciones seguras y consistentes, como la asignación de sensores, la confirmación de pagos o la renovación automática.

<img src="../img/subscription.png">

#### 4.2.1.2. Interface Layer.

En esta sección, se presenta la Capa de Interfaz de Subscription, la cual actúa como puente entre los usuarios y la lógica del dominio. Esta capa está compuesta por controladores que reciben solicitudes, las procesan y devuelven respuestas, facilitando una interacción clara y eficiente con la plataforma.

Los controladores principales incluyen:

SubscriptionController: Gestiona operaciones relacionadas con suscripciones, como creación, cancelación, renovación y asignación de sensores.

PaymentController: Se encarga del procesamiento de pagos, consulta de estados y confirmación o cancelación de transacciones.

<img src="../img/Controllers subsc.png">

#### 4.2.1.3. Application Layer.

En esta sección, se describe la Capa de Aplicación del sistema de Subscription, la cual actúa como intermediaria entre las solicitudes de la interfaz y la lógica de negocio del dominio. Esta capa se encarga de orquestar el flujo de operaciones, utilizando Command Handlers para ejecutar acciones específicas y coordinar los servicios necesarios.

Los componentes principales incluyen:

CreateSubscriptionCommandHandler: Gestiona la creación de suscripciones, delegando la lógica al SubscriptionService para garantizar que se cumplan las reglas de negocio.

ProcessPaymentCommandHandler: Coordina el procesamiento de pagos, interactuando con el PaymentService para validar y ejecutar transacciones.

<img src="../img/Application Layer subsc.png">

#### 4.2.1.4. Infrastructure Layer.

En esta sección, se detalla la Capa de Infraestructura del sistema de Subscription, la cual proporciona los componentes técnicos esenciales para la persistencia de datos y la integración con sistemas externos. Esta capa implementa los mecanismos de almacenamiento y recuperación de información, asegurando que el dominio y la aplicación operen sin preocuparse por los detalles técnicos subyacentes.

Los repositorios clave incluyen:

SubscriptionRepository: Encargado de gestionar las operaciones relacionadas con las suscripciones, como buscar por ID o residencial, guardar nuevos registros o eliminar suscripciones existentes.

PaymentRepository: Responsable de manejar los datos de pagos, permitiendo consultar transacciones por ID o suscripción, así como almacenar o eliminar información de pagos.

<img src="../img/Infrastructure Layer subsc.png">

#### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams.

#### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams.

##### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams.

<img src="../img/Layer Class Diagrams.png">

##### 4.2.1.6.2. Bounded Context Database Design Diagram.

<img src="../img/db design diagram subsc.png">

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
