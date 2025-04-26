# <center>COURSE PROJECT</center>

<p align="center">
    <strong>Universidad Peruana de Ciencias Aplicadas</strong><br>
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png"><br>
    <strong>Ingeniería de Software</strong><br>
    <strong>Desarrollo de Soluciones IOT - 2947</strong><br>
    <strong>Profesor: Angel Augusto Velasquez Nuñez </strong><br>
    <br>INFORME
</p>


<center>

#### Startup: **IronCoders**

#### Product: **AquaConecta**

</center>
# Team Members:

<div align="center">

|             Member                        |    Code      |
|:------------------------------------------|:------------:|
| Aguilar Castillo, Rodrigo                 | U202210584   |
| Carmelino Dueñas, Michael Stefano         | U202212760   |
| Cortez Quezada, Joaquin Antonio           | U202212648   |
| Párraga Gamarra, Paolo Gonzalo            | U202219186   |
| Periche Quiroga, Piero                    | U202210192   |
| Ramos Argüelles, Alexandra Belen          | U202215164   |


</div>

# Registro de Versiones del Informe

<div align="center">


| Versión | Fecha       | Autor                                     | Descripción de modificación                                                                                  |
|---------|-------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| TB1     | 3/04/2025    | Rodrigo Aguilar Castillo                 | Redacción inicial de antecedentes del proyecto y estructura base del documento.                             |
| TB1     | 5/04/2025    | Michael Stefano Carmelino Dueñas         | Desarrollo preliminar del modelo de arquitectura de componentes y flujos de usuarios.                       |
| TB1     | 8/04/2025    | Joaquin Antonio Cortez Quezada           | Revisión del mapeo de User Personas y adaptación de flujos de experiencia de usuario.                        |
| TB1     | 12/04/2025   | Paolo Gonzalo Párraga Gamarra             | Consolidación de entrevistas, hallazgos de usuarios y priorización de funcionalidades clave.                |
| TB1     | 18/04/2025   | Piero Periche Quiroga                    | Revisión del Lean UX Canvas y definición de métricas de éxito para el MVP inicial.                           |
| TB1     | 22/04/2025   | Alexandra Belen Ramos Argüelles          | Revisión final del documento, correcciones de redacción y generación de versión lista para entrega en PDF.   |




</div>

# Project Report Collaboration Insights

Repositorios:

Proyecto: [https://github.com/IronCoders-IOT/Final-Project](https://github.com/IronCoders-IOT/Final-Project)


### TB1

Para la entrega del TB1 se han realizado los procesos necesarios para lograr los objetivos propuestos de la entrega. Se toma en cuenta la importancia de la persistencia y como grupo nos dedicamos a mantener una frecuencia de commits y cambios proyectada a ser optima a futuro.

Se muestran evidencias de los commits realizados en la entrega de la TB1 en el informe.


[Colaboraciones del repositorio]

[Registro de los commits donde se realizaron la mayor cantidad]

En ambos casos se puede observar el incremento de modificaciones y revisiones en los dias miercoles y una cantidad mayor de cambios que commits.

---

# Contenido

[Registro de Versiones del Informe](#registro-de-versiones-del-informe)

[Project Report Collaboration Insights](#project-report-collaboration-insights)

[Student Outcome](#student-outcome)

[Capítulo I: Introducción](#capítulo-i-introducción)

[1.1 Startup Profile](#11-startup-profile)  
[1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)  
[1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)

[1.2. Solution Profile](#12-solution-profile)  
[1.2.1 Antecedentes y problemática](#121-antecedentes-y-problemática)  
[1.2.2 Lean UX Process.](#122-lean-ux-process)  
[1.2.2.1. Lean UX Problem Statements.](#1221-lean-ux-problem-statements)  
[1.2.2.2. Lean UX Assumptions.](#1222-lean-ux-assumptions)  
[1.2.2.3. Lean UX Hypothesis Statements.](#1223-lean-ux-hypothesis-statements)  
[1.2.2.4. Lean UX Canvas.](#1224-lean-ux-canvas)

[1.3. Segmentos objetivo.](#13-segmentos-objetivo)

[Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)

[2.1. Competidores](#21-competidores)  
[2.1.1. Análisis competitivo](#211-análisis-competitivo)  
[2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)

[2.2. Entrevistas](#22-entrevistas)  
[2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)    
[2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)

[2.3. Needfinding](#23-needfinding)  
[2.3.1. User Personas](#231-user-personas)  
[2.3.2. User Task Matrix](#232-user-task-matrix)  
[2.3.3. User Journey Mapping](#233-user-journey-mapping)  
[2.3.4. Empathy Mapping](#234-empathy-mapping)  
[2.3.5. As-is Scenario Mapping](#235-as-is-scenario-mapping)

[2.4. Ubiquitous Language](#24-ubiquitous-language)

[Capítulo III: Requirements Specifications](#capítulo-iii-requirements-specification)

[3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)

[3.2. User Stories](#32-user-stories)

[3.3. Impact Mapping](#33-impact-mapping)

[3.4. Product Backlog](#34-product-backlog)

[Capítulo IV: Solution Software Design](#capítulo-iv-solution-software-design)

[4.1. Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)   
[4.1.1. Event Storming](#411-event-storming)             
[4.1.1.1 Candidate Context Discovery](#4111-candidate-context-discovery)    
[4.1.1.2 Domain Message Flows Modeling](#4112-domain-message-flows-modeling)    
[4.1.1.3 Bounded Context Canvases](#4113-bounded-context-canvases)    
[4.1.2. Context Mapping](#412-context-mapping)    
[4.1.3. Software Architecture](#413-software-architecture)    
[4.1.3.1. Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram)        
[4.1.3.2. Software Architecture Context Level Diagrams](#4132-software-architecture-container-level-diagrams)      
[4.1.3.3. Software Architecture Deployment Diagrams](#4133-software-architecture-deployment-diagrams)      
[4.2. Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design)       

[4.2.1. Bounded Context: Management](#421-bounded-context-management)   
[4.2.1.1. Domain Layer](#4211-domain-layer)    
[4.2.1.2. Interface Layer](#4212-interface-layer)    
[4.2.1.3. Application Layer](#4213-application-layer)    
[4.2.1.4. Infrastructure Layer](#4214-infrastructure-layer)    
[4.2.1.5. Bounded Context Software Architecture Component Level Diagrams](#4215-bounded-context-software-architecture-component-level-diagrams)     
[4.2.1.6. Bounded Context Software Architecture Code Level Diagrams](#4216-bounded-context-software-architecture-code-level-diagrams)     
[4.2.1.6.1. Bounded Context Domain Layer Class Diagrams](#42161-bounded-context-domain-layer-class-diagrams)      
[4.2.1.6.2. Bounded Context Database Design Diagram](#42162-bounded-context-database-design-diagram)      

[4.2.2. Bounded Context: Analytics](#422-bounded-context-analytics)    
[4.2.2.1. Domain Layer](#4221-domain-layer)    
[4.2.2.2. Interface Layer](#4222-interface-layer)    
[4.2.2.3. Application Layer](#4223-application-layer)    
[4.2.2.4. Infrastructure Layer](#4224-infrastructure-layer)    
[4.2.2.5. Bounded Context Software Architecture Component Level Diagrams](#4225-bounded-context-software-architecture-component-level-diagrams)    
[4.2.2.6. Bounded Context Software Architecture Code Level Diagrams](#4226-bounded-context-software-architecture-code-level-diagrams)    
[4.2.2.6.1. Bounded Context Domain Layer Class Diagrams](#42261-bounded-context-domain-layer-class-diagrams)    
[4.2.2.6.2. Bounded Context Database Design Diagram](#42262-bounded-context-database-design-diagram)     

[4.2.3. Bounded Context: Consulting](#423-bounded-context-consulting)     
[4.2.3.1. Domain Layer](#4231-domain-layer)     
[4.2.3.2. Interface Layer](#4232-interface-layer)     
[4.2.3.3. Application Layer](#4233-application-layer)    
[4.2.3.4. Infrastructure Layer](#4234-infrastructure-layer)    
[4.2.3.5. Bounded Context Software Architecture Component Level Diagrams](#4235-bounded-context-software-architecture-component-level-diagrams)    
[4.2.3.6. Bounded Context Software Architecture Code Level Diagrams](#4236-bounded-context-software-architecture-code-level-diagrams)    
[4.2.3.6.1. Bounded Context Domain Layer Class Diagrams](#42361-bounded-context-domain-layer-class-diagrams)     
[4.2.3.6.2. Bounded Context Database Design Diagram](#42362-bounded-context-database-design-diagram)      

[4.2.4. Bounded Context: Subscription](#424-bounded-context-subscription)     
[4.2.4.1. Domain Layer](#4241-domain-layer)     
[4.2.4.2. Interface Layer](#4242-interface-layer)     
[4.2.4.3. Application Layer](#4243-application-layer)    
[4.2.4.4. Infrastructure Layer](#4244-infrastructure-layer)    
[4.2.4.5. Bounded Context Software Architecture Component Level Diagrams](#4245-bounded-context-software-architecture-component-level-diagrams)    
[4.2.4.6. Bounded Context Software Architecture Code Level Diagrams](#4246-bounded-context-software-architecture-code-level-diagrams)    
[4.2.4.6.1. Bounded Context Domain Layer Class Diagrams](#42461-bounded-context-domain-layer-class-diagrams)    
[4.2.4.6.2. Bounded Context Database Design Diagram](#42462-bounded-context-database-design-diagram)    

[4.2.5. Bounded Context: Payment](#425-bounded-context-payment)    
[4.2.5.1. Domain Layer](#4251-domain-layer)    
[4.2.5.2. Interface Layer](#4252-interface-layer)    
[4.2.5.3. Application Layer](#4253-application-layer)    
[4.2.5.4. Infrastructure Layer](#4254-infrastructure-layer)    
[4.2.5.5. Bounded Context Software Architecture Component Level Diagrams](#4255-bounded-context-software-architecture-component-level-diagrams)    
[4.2.5.6. Bounded Context Software Architecture Code Level Diagrams](#4256-bounded-context-software-architecture-code-level-diagrams)    
[4.2.5.6.1. Bounded Context Domain Layer Class Diagrams](#42561-bounded-context-domain-layer-class-diagrams)    
[4.2.5.6.2. Bounded Context Database Design Diagram](#42562-bounded-context-database-design-diagram)     

[4.2.6. Bounded Context: Automation](#426-bounded-context-automation)    
[4.2.6.1. Domain Layer](#4261-domain-layer)     
[4.2.6.2. Interface Layer](#4262-interface-layer)     
[4.2.6.3. Application Layer](#4263-application-layer)    
[4.2.6.4. Infrastructure Layer](#4264-infrastructure-layer)    
[4.2.6.5. Bounded Context Software Architecture Component Level Diagrams](#4265-bounded-context-software-architecture-component-level-diagrams)    
[4.2.6.6. Bounded Context Software Architecture Code Level Diagrams](#4266-bounded-context-software-architecture-code-level-diagrams)    
[4.2.6.6.1. Bounded Context Domain Layer Class Diagrams](#42661-bounded-context-domain-layer-class-diagrams)    
[4.2.6.6.2. Bounded Context Database Design Diagram](#42662-bounded-context-database-design-diagram)     

[4.2.7. Bounded Context: Installation](#427-bounded-context-installation)     
[4.2.7.1. Domain Layer](#4271-domain-layer)     
[4.2.7.2. Interface Layer](#4272-interface-layer)     
[4.2.7.3. Application Layer](#4273-application-layer)     
[4.2.7.4. Infrastructure Layer](#4274-infrastructure-layer)     
[4.2.7.5. Bounded Context Software Architecture Component Level Diagrams](#4275-bounded-context-software-architecture-component-level-diagrams)     
[4.2.7.6. Bounded Context Software Architecture Code Level Diagrams](#4276-bounded-context-software-architecture-code-level-diagrams)     
[4.2.7.6.1. Bounded Context Domain Layer Class Diagrams](#42761-bounded-context-domain-layer-class-diagrams)     
[4.2.7.6.2. Bounded Context Database Design Diagram](#42762-bounded-context-database-design-diagram)     

[4.2.8. Bounded Context: Identity and Access Management](#428-bounded-context-identity-and-access-management)     
[4.2.8.1. Domain Layer](#4281-domain-layer)     
[4.2.8.2. Interface Layer](#4282-interface-layer)     
[4.2.8.3. Application Layer](#4283-application-layer)     
[4.2.8.4. Infrastructure Layer](#4284-infrastructure-layer)     
[4.2.8.5. Bounded Context Software Architecture Component Level Diagrams](#4285-bounded-context-software-architecture-component-level-diagrams)     
[4.2.8.6. Bounded Context Software Architecture Code Level Diagrams](#4286-bounded-context-software-architecture-code-level-diagrams)     
[4.2.8.6.1. Bounded Context Domain Layer Class Diagrams](#42861-bounded-context-domain-layer-class-diagrams)     
[4.2.8.6.2. Bounded Context Database Design Diagram](#42862-bounded-context-database-design-diagram)     

[4.2.9. Bounded Context: Notifications](#429-bounded-context-notifications)     
[4.2.9.1. Domain Layer](#4291-domain-layer)     
[4.2.9.2. Interface Layer](#4292-interface-layer)     
[4.2.9.3. Application Layer](#4293-application-layer)     
[4.2.9.4. Infrastructure Layer](#4294-infrastructure-layer)     
[4.2.9.5. Bounded Context Software Architecture Component Level Diagrams](#4295-bounded-context-software-architecture-component-level-diagrams)     
[4.2.9.6. Bounded Context Software Architecture Code Level Diagrams](#4296-bounded-context-software-architecture-code-level-diagrams)     
[4.2.9.6.1. Bounded Context Domain Layer Class Diagrams](#42961-bounded-context-domain-layer-class-diagrams)     
[4.2.9.6.2. Bounded Context Database Design Diagram](#42962-bounded-context-database-design-diagram)     
             

[Conclusiones](#conclusiones)

[Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)

[Video About-the-Team](#video-about-the-team)

[Bibliografía](#bibliografía)

[Anexos](#anexos)

# Student Outcome
El curso contribuye al cumplimiento del Student Outcome ABET:
ABET – EAC - Student Outcome 5
Criterio: La capacidad de funcionar efectivamente en un equipo cuyos miembros
juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo,
establecen objetivos, planifican tareas y cumplen objetivos.
En el siguiente cuadro se describe las acciones realizadas y enunciados de
conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro
del ABET – EAC - Student Outcome 5.

| **Criterio Específico** | **Acciones Realizadas** | **Conclusiones** |
|-------------------------|-------------------------|------------------|
| Trabaja en equipo para proporcionar liderazgo en forma conjunta | **Alexandra Belen Ramos Argüelles** <br>**TB1:**<br> Lideré la organización del equipo en el proyecto AquaConecta, coordinando las reuniones, la definición de la estrategia de trabajo, y la organización de entregables. Supervisé los avances del event storming, la construcción de User Personas, la elaboración del Lean UX Canvas y el modelado de los principales diagramas técnicos, asegurando una visión integrada de todo el proyecto. <br><br> **Rodrigo Aguilar Castillo** <br>**TB1:**<br> Participé en la definición del flujo de usuarios, contribuyendo en la elaboración de los diagramas de interacción y apoyando en el diseño de la arquitectura de capas, especialmente en la identificación de servicios críticos como la gestión de sensores y eventos de AquaConecta. <br><br> **Michael Stefano Carmelino Dueñas** <br>**TB1:**<br> Aporté en el desarrollo del Context Map general del sistema, ayudando en la identificación de Bounded Contexts y trabajando en la definición técnica de los principales aggregates para la plataforma. También colaboré en la elaboración de los primeros esquemas de la base de datos relacional. <br><br> **Joaquin Antonio Cortez Quezada** <br>**TB1:**<br> Trabajé activamente en la definición de User Personas y en la identificación de segmentos de usuario (hogares, agricultores, técnicos). Además, participé en la construcción de los flujos de experiencia iniciales y en el diseño del User Journey Mapping. <br><br> **Paolo Gonzalo Párraga Gamarra** <br>**TB1:**<br> Colaboré en el levantamiento de eventos de negocio durante las sesiones de event storming, apoyando además en la priorización de funcionalidades esenciales para el MVP y en la validación de los flujos de interacción usuario-sistema. <br><br> **Piero Periche Quiroga** <br>**TB1:**<br> Participé en la validación técnica de los diagramas generados (Bounded Contexts, Arquitectura de Capas y Componentes), asegurando su consistencia con los requerimientos levantados y apoyando en la revisión de las entrevistas realizadas a los segmentos objetivo. | El equipo demostró un liderazgo conjunto sólido, con Alexandra coordinando las acciones principales y cada integrante contribuyendo activamente al desarrollo de flujos, levantamiento de eventos, diseño técnico, experiencia de usuario y validación de artefactos. Se logró un avance integral del proyecto AquaConecta de manera organizada y colaborativa. |
| Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos. | **Alexandra Belen Ramos Argüelles** <br>**TB1:**<br> Organicé y supervisé la planificación de tareas por etapas, estableciendo metas semanales claras y promoviendo espacios de discusión abiertos para garantizar la participación de todos los miembros en la toma de decisiones clave. <br><br> **Rodrigo Aguilar Castillo** <br>**TB1:**<br> Participé en la coordinación de actividades técnicas, ayudando a definir prioridades en el diseño de flujos de usuario y contribuyendo a mantener la comunicación constante entre todos los miembros durante la construcción de diagramas técnicos. <br><br> **Michael Stefano Carmelino Dueñas** <br>**TB1:**<br> Apoyé en la definición de objetivos técnicos semanales relacionados a la creación del Context Map y Bounded Context Canvas, facilitando la validación cruzada de entregables entre los integrantes. <br><br> **Joaquin Antonio Cortez Quezada** <br>**TB1:**<br> Colaboré activamente en las sesiones de planificación de funcionalidades desde la perspectiva del usuario, asegurando que las metas de experiencia de usuario y segmentación fueran contempladas en todas las decisiones estratégicas. <br><br> **Paolo Gonzalo Párraga Gamarra** <br>**TB1:**<br> Aporté a la organización y priorización de tareas derivadas del event storming y participé en la planificación de las actividades relacionadas a la identificación de eventos críticos del sistema. <br><br> **Piero Periche Quiroga** <br>**TB1:**<br> Contribuí en la planificación y validación de entregables parciales como diagramas técnicos y flujos de usuario, asegurando la correcta alineación de los entregables con los objetivos del proyecto definidos en las reuniones grupales. | Gracias al liderazgo colaborativo y la participación activa de todos los integrantes, se logró establecer un entorno de trabajo inclusivo, con metas claras y planificación efectiva que garantizó el cumplimiento de los entregables y la calidad de los resultados obtenidos en AquaConecta.

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

AquaConecta es una empresa emergente que se destaca por su enfoque innovador en la implementación de soluciones IoT para optimizar el acceso y la distribución de agua potable. Fundada con el propósito de mejorar la gestión del suministro en comunidades que no cuentan con un servicio continuo, AquaConecta ha logrado posicionarse como un actor clave en el sector gracias a su capacidad para desarrollar plataformas tecnológicas que conectan a proveedores de agua con usuarios finales de manera eficiente y transparente. <br><br>

Nuestra empresa se caracteriza por su compromiso con la innovación, la sostenibilidad y el impacto social. En AquaConecta, creemos firmemente en el poder de la tecnología para transformar la forma en que las personas acceden a recursos esenciales. Por ello, nos enfocamos en ofrecer soluciones inteligentes que permitan monitorear en tiempo real la calidad y cantidad del agua, mejorando la toma de decisiones tanto para proveedores como para usuarios.<br><br>

Como empresa emergente, estamos comprometidos con un crecimiento sostenible y con la expansión de nuestro alcance tanto a nivel nacional como internacional. Nos enorgullece ser parte de una revolución tecnológica en la gestión del agua potable, y estamos entusiasmados por seguir desarrollando herramientas que promuevan una distribución más justa, eficiente y segura mediante nuestra tecnología IoT avanzada

#### Visión

La visión de AquaConecta es ser líder en soluciones IoT para el acceso y distribución eficiente de agua potable, ofreciendo tecnología de vanguardia que garantice la calidad, disponibilidad y gestión inteligente del recurso hídrico en comunidades de todo el mundo.

#### Misión

La misión de AquaConecta es desarrollar y ofrecer soluciones tecnológicas basadas en IoT que mejoren el acceso al agua potable, facilitando la conexión entre proveedores y comunidades sin suministro continuo, mediante herramientas que garanticen una distribución eficiente, transparente y sostenible.

### 1.1.2. Perfiles de los integrantes

| Nombre                   | Descripción | Foto |
|--------------------------|-------------|------|
| Rodrigo Aguilar Castillo | Soy Rodrigo, estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC). Me apasiona la tecnología y los dispositivos electrónicos, y disfruto especialmente programar, lo cual se ha convertido en uno de mis principales pasatiempos.<br>Siempre estoy buscando aprender nuevas herramientas y mejorar mis habilidades en el desarrollo de software.<br><br>**Habilidades Técnicas**<br>- Desarrollo Frontend con **Angular** y **Vue**<br>- Desarrollo Backend con **Java** y **Spring Boot**<br>- Conocimientos en **C++**<br>- Manejo intermedio de **SQL** |<img src="./img/rodrigo_aguilar.png" width="350" height="150"> |
| Paolo Gonzalo Párraga Gamarra | Soy Paolo Párraga, estudiante de ingeniería de software en séptimo ciclo. Soy una persona que disfruta trabajar duro para lograr mis objetivos y nunca me rindo a pesar de los momentos difíciles. Me gusta el trabajo en equipo porque siento que puedo aportar a mis compañeros cuando lo necesiten.<br><br>**Habilidades Técnicas**<br>- Desarrollo Frontend con **Angular** y **Vue**<br>- Desarrollo Backend con **Java** y **Spring Boot**<br>- Conocimientos en **C++**<br>- Manejo intermedio de **SQL** |<img src="./img/PaoloParraga.jfif" width="350" height="170"> |
| Alexandra Belen Ramos Argüelles | Soy Alexandra Ramos, estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC), actualmente cursando el séptimo ciclo. Me considero una persona empática, responsable y perseverante. Disfruto trabajar en equipo y me adapto con facilidad a distintos entornos de colaboración. Creo firmemente que la comunicación asertiva y el apoyo mutuo son claves para alcanzar resultados significativos. <br><br>Me apasiona desarrollar soluciones tecnológicas que generen un impacto positivo en la sociedad, especialmente en contextos donde la innovación puede marcar la diferencia. <br><br>**Habilidades Técnicas**<br>- Desarrollo Frontend con **Angular** y **Vue**. <br>- Desarrollo Backend con **Java** y **Spring Boot**.<br>- Conocimientos en **C++**, **C#** y **Python**. | <img src="./img/alexandra_ramos.jfif" widht="350" height="155">
| Michael Stefano Carmelino Dueñas | Soy Michael Carmelino, estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC), actualmente cursando el séptimo ciclo. Soy una persona que le gusta el trabajo en equipo donde haya una comunicación y formas de integrarse entre todos para llegar a un fin común. <br><br>Me gusta desarrollar proyectos que tengan que ver con la seguridad en ciertos aspectos pero también me gusta hacer proyectos que me den a mi facilidades en lo personal o por diversión. <br><br>**Habilidades Técnicas**<br>- Desarrollo Frontend con **React** y **Tailwind**. <br>- Desarrollo Backend con **Nest Js ** y **Spring Boot**.<br>- Conocimientos en **C++**, **Python** y **Java**. <br> - Base de datos con **Supabase**| <img src="./img/michaelcarmelino.jpg" widht="350" height="155">
| Joaquin Antonio Cortez Quezada | Soy Joaquin Antonio Cortez Quezada, actualmente estoy cursando el séptimo ciclo de la carrera de Ingeniería de Software en la UPC (Universidad Peruana de Ciencias Aplicadas). Me considero una persona perseverante, responsable, con la capacidad de aprender y adaptarme de forma rápida enfrentar diversos desafíos tecnológicos.  <br><br>**Habilidades Técnicas**<br>- Desarrollo Frontend con Angular y Vue <br>- Desarrollo Backend con Java y Spring Boot<br>- Conocimientos en C++, Python <br>- Manejo intermedio de MySQL, PostgreSQL| <img src="./img/cortezquezadaimg.jpeg" widht="350" height="155">
| Piero Fernando Periche Quiroga | Soy Piero Fernando Periche Quiroga, estoy cursando el 7timo ciclo de la carrerar de Ingerniería de Software en la UPC, soy una persona responsable, perseverante y con la capacidad de aprender y poder aportar buenas ideas al equipo frente a los problemas que se puedan presentar. <br><br> **Habilidades Técnicas**<br> - Desarrollo frontend con Vue y Angular <br> - Desarrollo de backend con java y c# <br>- Conocimiento de MYSQL Y MongoDB | ![Imagen del compañero](https://i.imgur.com/IIMIR5W.jpeg)

<!---Falta piero stefano------->


## 1.2. Solution Profile

AquaConecta nace como respuesta a la necesidad de mejorar el acceso y la distribución de agua potable en comunidades sin suministro constante. A través de una plataforma inteligente con tecnología IoT, conecta a proveedores con usuarios, permitiendo monitorear en tiempo real la calidad y cantidad del agua disponible.

Gracias a sus sensores y acceso desde dispositivos móviles o web, la solución facilita la planificación de rutas de distribución y brinda a los usuarios control total sobre su consumo. Su enfoque automatizado, accesible y centrado en datos la convierte en una herramienta eficiente para optimizar la gestión del agua y generar un impacto positivo en la calidad de vida de las personas.

### 1.2.1. Antecedentes y problemática

En regiones como **Ica y Chincha**, miles de familias enfrentan una grave crisis de acceso al agua potable, ya que solo el **13.3% de los hogares** cuentan con suministro continuo durante las 24 horas del día ([Infobae, 2024](https://www.infobae.com/peru/2024/09/08/alarma-por-la-falta-de-acceso-continuo-a-agua-potable-en-ica-solo-el-133-de-los-hogares-cuenta-con-el-servicio-las-24-horas/?utm_source=chatgpt.com)). Ante esta situación, muchas personas dependen del abastecimiento mediante **camiones cisterna**, lo cual resuelve de forma temporal la necesidad, pero genera nuevos desafíos en la gestión y control del recurso. A pesar de los esfuerzos de empresas como **Semapach** y la supervisión de organismos como **Sunass**, se identifican diversos problemas estructurales que dificultan una distribución justa y segura del agua.

#### Principales problemáticas identificadas:

- **Falta de trazabilidad y control por vivienda:** no hay un registro automatizado de cuánta agua se entrega a cada familia.  
- **Distribución ineficiente:** algunas zonas no reciben agua a tiempo o quedan fuera de la planificación.  
- **Riesgos en la calidad del agua:** no siempre se verifica si el agua distribuida por cisterna cumple los estándares de salubridad.  
- **Dependencia de métodos manuales:** muchas decisiones logísticas se toman sin apoyo de datos en tiempo real.  
- **Problemas sanitarios:** el almacenamiento en baldes o tanques sin tapa incrementa el riesgo de enfermedades como el dengue.  

Esta realidad evidencia la necesidad de adoptar soluciones tecnológicas, como sistemas de monitoreo IoT y plataformas digitales de gestión, que permitan optimizar el reparto, mejorar la transparencia y garantizar la calidad del agua entregada.


AquaConecta surge como una solución integral para enfrentar los desafíos en la distribución y gestión del agua potable en comunidades sin acceso continuo al servicio. Esta plataforma inteligente, basada en tecnología IoT, permite a las empresas proveedoras monitorear en tiempo real la calidad y cantidad de agua disponible directamente desde los tanques de almacenamiento en las viviendas, lo que mejora significativamente la trazabilidad y eficiencia del servicio.

Gracias a sensores instalados en cada tanque, se recopilan datos sobre niveles de agua, posibles contaminantes y consumo, los cuales son transmitidos a una aplicación web y móvil. Esto brinda a los usuarios finales información clara sobre su suministro, y a los proveedores una herramienta poderosa para planificar rutas de abastecimiento, priorizar zonas críticas y tomar decisiones basadas en datos reales.

Con AquaConecta, se optimiza la distribución, se reducen los riesgos sanitarios asociados al almacenamiento inseguro y se garantiza un uso más inteligente y equitativo del recurso hídrico. Esta solución no solo responde a una necesidad urgente, sino que también impulsa la transformación digital de los servicios de agua, promoviendo un acceso más justo, transparente y sostenible para todos.



#### Técnica de las 5W's y 2H's

##### ¿What? - ¿Cuál es el problema?

 Falta de control y visibilidad sobre el agua en tanques domésticos, lo que impide a las familias saber cuánta agua tienen y su calidad, y a los proveedores gestionar eficientemente las entregas.

##### ¿Who? - ¿Quienes son los beneficiarios?

 Las familias sin acceso continuo a agua potable y los proveedores de agua como empresas, municipalidades y ONGs que buscan optimizar la distribución y monitoreo del recurso.

 ##### ¿When? - ¿Cuando se origina el problema?
 El problema se origina de forma continua, especialmente cuando no hay acceso constante al agua potable, durante cortes inesperados, épocas de sequía o cuando el usuario no puede supervisar manualmente el estado del agua almacenada.

##### ¿Why? - ¿Por qué se origina el problema?

El problema se origina por el acceso limitado o intermitente al agua potable y la falta de control sobre su almacenamiento, lo que dificulta una distribución eficiente y transparente.

##### ¿Where? - ¿Dónde ocurre el problema?

El problema ocurre en hogares y comunidades de zonas urbanas periféricas y rurales con acceso limitado al agua, como Ica y Chincha, donde se depende de tanques y camiones cisterna para el abastecimiento.


##### ¿How? - ¿Como se origina el problema?

El problema se origina por la falta de visibilidad sobre el nivel y la calidad del agua en los tanques, debido a la ausencia de herramientas que permitan monitoreo continuo y acceso a información en tiempo real. Esto genera ineficiencia, desperdicio y desinformación.

##### ¿How much? - ¿Cuánto dinero está implicado?

AquaConecta ofrece planes mensuales entre S/500 y S/1,000, según la cantidad de usuarios que la empresa de agua gestione, e incluye monitoreo y gestión en tiempo real.
 
---                                                                                            
### 1.2.2 Lean UX Process.

El proceso Lean UX aborda la visión del modelo de negocio que respalda nuestro proyecto, siendo el producto principal nuestro software. A lo largo de este documento y en este capítulo, exploramos varios elementos clave de este proceso.

Comenzamos con los "Problem Statements", que abarcan aspectos como el dominio, los segmentos de clientes, los puntos de dolor, las brechas, la visión/estrategia y el segmento inicial. Siguiendo la metodología Lean UX, también consideramos las "Assumptions Statements" y las "Hypothesis Statements".

#### 1.2.2.1. Lean UX Problem Statements.

**Problem Statement:**
### Lean UX Problem Statement – AquaConecta

En muchas zonas rurales, las comunidades enfrentan un acceso limitado al agua potable debido a una distribución ineficiente y a la falta de información sobre la calidad del agua que consumen. Esta situación pone en riesgo la salud de las personas y dificulta una adecuada gestión del recurso hídrico. Sin un monitoreo continuo y preciso, se vuelve imposible identificar fugas, optimizar el suministro o tomar decisiones informadas para garantizar un servicio equitativo y seguro.

Actualmente no existen mecanismos efectivos ni tecnologías accesibles que permitan monitorear en tiempo real tanto la calidad como la cantidad del agua distribuida. Las soluciones disponibles suelen ser costosas, de difícil implementación en zonas con baja conectividad, o no están adaptadas al contexto rural y comunitario, lo que impide su adopción y sostenibilidad.

AquaConecta se enfoca en ofrecer un sistema integral de monitoreo del recurso hídrico basado en tecnología IoT, diseñado para empoderar a los gestores comunitarios del agua con datos claros y en tiempo real. Esta solución facilita una toma de decisiones más eficiente, transparente y orientada a la sostenibilidad del servicio.

Nuestra plataforma combina sensores para medir caudal, presión y parámetros de calidad del agua. A través de un dashboard centralizado, los usuarios pueden visualizar alertas, generar reportes y tomar decisiones informadas sobre la gestión del agua.

Como resultado, nos enfrentamos al siguiente problema: ¿Cómo podemos proveer una plataforma de monitoreo del recurso hídrico que permita reducir en un 40% el tiempo de respuesta ante fallos, mejorar la calidad del agua distribuida y aumentar la eficiencia operativa en comunidades rurales?

El sistema está pensado para implementarse en comunidades rurales y zonas de alta vulnerabilidad, apoyando tanto a municipalidades, ONGs y líderes comunitarios como a instituciones académicas y proyectos de desarrollo sostenible.

Sabremos que hemos tenido éxito cuando al menos el 50% de las comunidades intervenidas reporten una mejora del 40% en eficiencia operativa, reducción de fugas o mejora percibida en la calidad del agua, según encuestas de seguimiento y métricas recopiladas por la plataforma.

---

#### 1.2.2.2. Lean UX Assumptions.

En esta sección, veremos los Assumptions que podemos esperar de nuestra solución, desde los Features que debe tener, hasta los Outcomes en nuestra perspectiva y la de los usuarios.

**Features:**

Aqui veremos las herramientas que planeamos implementar en nuestra solución.

- Monitoreo en Tiempo Real de Calidad y Cantidad de Agua: Sensores IoT que recopilan datos sobre el caudal, presión, nivel de cloro, turbidez, entre otros parámetros del agua, enviando la información a una plataforma centralizada.
- Alertas Automatizadas: Notificaciones en tiempo real sobre anomalías en la calidad del agua o interrupciones en el suministro, dirigidas a autoridades locales, técnicos o responsables comunitarios.
- Dashboard Centralizado de Datos: Plataforma accesible desde dispositivos móviles o PC para visualizar gráficamente el estado del suministro, históricos y predicciones de comportamiento hídrico.
- Reportes Automáticos para Toma de Decisiones: Generación de reportes periódicos para los tomadores de decisiones, con métricas claves para planificación y mejora de la infraestructura.

**Business Outcomes:**

Acquisition (Base): [3,000 visitantes]
Las comunidades rurales, organizaciones sociales y municipalidades se enteran de nuestra solución a través de campañas en redes sociales, ferias tecnológicas rurales, charlas con ONGs y contenido educativo. Además, se realizarán alianzas con entidades públicas y privadas que promuevan la transformación digital en zonas rurales. Estimamos alcanzar inicialmente a 3,000 personas interesadas en el tema de gestión del agua.

Activation (Plateau): [900 usuarios : 100%]
De los visitantes, se espera que el 30% (900 usuarios) participen activamente en una demostración del sistema o soliciten un diagnóstico gratuito para su comunidad. En esta fase, los usuarios nos comparten información básica como ubicación de su sistema de agua, número de conexiones, tipo de infraestructura y principales problemas. También acceden por primera vez a nuestra plataforma con credenciales temporales.

Retention (Plateau + 1 level): [540 usuarios : 60%]
Tras la activación, un 60% de las comunidades implementan el sistema de manera continua y lo usan para monitorear su infraestructura hídrica. Estas comunidades acceden regularmente a los datos del sistema, reciben alertas automáticas y visualizan mejoras progresivas en su servicio, lo que incentiva el uso constante. Aquí se empieza a notar la reducción del 40% en interrupciones y se ve reflejada la mejora del 25% en la calidad del agua, validando la funcionalidad del producto.

Revenue (Plateau + 2 levels): [80 usuarios : ~15%]
De los usuarios retenidos, se proyecta que al menos el 15% opte por un plan de monitoreo avanzado, que incluye mantenimiento predictivo, personalización de alertas y análisis más profundo de los datos. Este grupo valora la capacidad del sistema para reducir un 30% los costos de operación, y está dispuesto a pagar por estas funcionalidades premium.

Referral (Top): [27 usuarios : 5% del total inicial]
Un 5% de los usuarios referirán nuestra solución a otras comunidades, ONGs o municipios, gracias a su experiencia positiva. Estos promotores naturales ayudan a amplificar nuestro alcance de forma orgánica, aportando nuevas oportunidades de implementación y reforzando nuestra posición como referente en soluciones IoT para zonas rurales.



## Users

En esta sección creamos un Proto-Persona como una suposición de cómo son nuestros usuarios, enfocándonos más en el aspecto de actitud.

| Demográfica                                   | Comportamiento                                                                                          | Necesidades / Obstáculos                                                                                      |
|----------------------------------------------|----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Gestores de Agua Rurales:                    | - Supervisan el sistema de distribución de agua de toda una comunidad                                     | - Necesitan visibilidad total del estado del sistema hídrico                                                   |
| Municipalidad, ONG, Junta de usuarios        | - Tienen experiencia gestionando recursos públicos o sociales                                             | - Requieren reportes detallados para tomar decisiones técnicas y presupuestales                               |
|                                              | - Se enfrentan constantemente a reclamos por fallas o baja calidad del agua                               | - Necesitan detectar fallas rápidamente para reducir tiempos de respuesta e interrupciones                    |
|                                              | - Buscan optimizar los recursos disponibles y generar confianza con la comunidad                          | - Buscan fortalecer la transparencia y generar reportes públicos                                               |
| Personas en zonas vulnerables:               | - Sufren cortes de agua frecuentes o reciben agua de baja calidad                                         | - Quieren saber si el agua que consumen es segura para su familia                                              |
| Residentes de comunidades rurales            | - No cuentan con acceso directo a la gestión del agua                                                     | - Necesitan una forma accesible para reportar fallas o problemas                                                |
|                                              | - Se enteran de las fallas solo cuando el problema ya está avanzado                                       | - Buscan tener más información sobre lo que sucede con el servicio de agua                                     |
|                                              | - Participan en asambleas o reuniones comunales para expresar sus necesidades                             | - Necesitan confiar en los gestores del agua y saber que sus necesidades están siendo atendidas               |

## User Outcomes & Benefits **


En esta sección se busca el lado más emocional y empatizar con el usuario para darles los outcomes correctos.

**¿Qué busca lograr el usuario?**
Asegurar el acceso a agua segura y confiable para su comunidad, y mejorar la eficiencia en la gestión del recurso hídrico.

**¿Cómo se quiere sentir el usuario en este proceso?**
Tranquilo, empoderado y respaldado por información clara que le permita tomar decisiones oportunas sin depender únicamente de inspecciones manuales.

**¿Cómo nuestro producto acerca al usuario a un logro personal?**
La solución IoT le proporciona datos en tiempo real sobre la calidad del agua, lo que le permite anticiparse a problemas y demostrar su capacidad de liderazgo en la comunidad.

**¿Por qué nuestro usuario buscaría nuestro producto?**
Porque necesita una herramienta que le facilite detectar a tiempo problemas de contaminación o fallas en la red de distribución, sin requerir grandes conocimientos técnicos ni inversiones costosas.

**¿Qué cambio de comportamiento podemos observar que nos cuente que lograron su objetivo?**
El usuario consulta la plataforma con frecuencia, responde más rápido a eventos anómalos, informa mejor a su comunidad y optimiza el uso de recursos en la gestión del agua.

Solutions
A partir de los problemas detectados en las entrevistas y el contexto rural, proponemos las siguientes soluciones tecnológicas:


- Monitoreo de calidad del agua (pH, turbidez, temperatura):

Problema: Las comunidades no tienen forma de detectar a tiempo si el agua está contaminada.

Solución: Sensores que miden en tiempo real parámetros como pH, turbidez y temperatura del agua.

Resultado: El sistema emite alertas inmediatas si se detecta contaminación, lo que permite prevenir enfermedades y mejorar la salud pública.

- Alertas automáticas ante condiciones críticas:

Problema: La falta de monitoreo continuo genera respuestas tardías ante emergencias sanitarias.

Solución: Plataforma que notifica automáticamente a los gestores mediante SMS o app cuando se detectan valores anómalos.

Resultado: Reducción significativa del tiempo de reacción ante problemas, lo que minimiza riesgos sanitarios.

- Panel de control comunitario:

Problema: Los gestores y ciudadanos no tienen acceso a información visual y clara sobre el estado del agua.

Solución: Dashboard con indicadores simples y accesibles (semáforo de calidad, gráficas por día, semana y mes).

Resultado: Mejora de la transparencia, empoderamiento ciudadano y participación comunitaria en el cuidado del agua.

- Historial de datos y reportes automáticos:

Problema: No se cuenta con registros para evaluar tendencias o realizar auditorías.

Solución: Almacenamiento de datos históricos accesibles en cualquier momento y generación de reportes descargables.

Resultado: Mejora de la planificación, mantenimiento predictivo e informes técnicos para autoridades o donantes.

- Funcionalidad offline y bajo consumo energético:

Problema: En zonas remotas no hay conectividad constante ni acceso a energía eléctrica.

Solución: Uso de sensores con batería solar, comunicación vía redes LoRa o GSM y almacenamiento local en el dispositivo.

Resultado: Asegura la continuidad del monitoreo en cualquier entorno, incluso sin internet.



**Business Assumptions:**

Estos son los puntos que podemos asumir de nuestro negocio.

1. Existe una necesidad urgente de mejorar la gestión del agua en zonas rurales, especialmente en lugaers en vías de desarrollo.
2. Esta necesidad puede resolverse con una solución IoT accesible, autónoma y fácil de usar por personal técnico o líderes comunitarios.
3. El valor principal que buscan los clientes es una forma confiable y económica de monitorear y mejorar el sistema hídrico sin requerir grandes inversiones.
4. Nuestros clientes potenciales serán principalmente gobiernos locales, ONGs, cooperativas y empresas sociales con foco en desarrollo rural.
5. Obtendremos ingresos a través de un modelo mixto: venta de kits IoT + suscripción a la plataforma de monitoreo, con opciones de personalización e integración.
6. Aunque existen soluciones similares, muchas son costosas o complejas. Nuestra ventaja está en la adaptabilidad, escalabilidad y soporte local.
7. El mayor riesgo es la falta de conectividad o acceso a tecnologías en zonas remotas.
8. Planeamos mitigar este riesgo mediante tecnologías de bajo consumo energético, almacenamiento offline y comunicación vía redes alternativas (LoRa, GSM, etc.).



#### 1.2.2.3. Lean UX Hypothesis Statements.
### Hipótesis del Proyecto

- **Hipótesis 1:**  
  Creemos que lograremos el posicionamiento como referentes en soluciones IoT para comunidades rurales,  
  si los gestores de agua obtienen una experiencia clara y visualmente intuitiva mediante el uso del dashboard centralizado de datos.

- **Hipótesis 2:**  
  Creemos que obtendremos una mejora significativa en la eficiencia operativa,  
  si los técnicos de mantenimiento reciben alertas automatizadas en tiempo real ante problemas en el sistema de distribución de agua.

- **Hipótesis 3:**  
  Creemos que se logrará una mejora en la calidad del agua distribuida,  
  si los gestores de agua pueden monitorear constantemente parámetros como turbidez, cloro y presión a través de los sensores IoT instalados.

- **Hipótesis 4:**  
  Creemos que se reducirá el tiempo de respuesta ante incidentes,  
  si los técnicos y responsables locales reciben notificaciones inmediatas mediante el sistema de alertas inteligentes.

- **Hipótesis 5:**  
  Creemos que la transparencia y la confianza comunitaria aumentarán,  
  si los líderes comunitarios tienen acceso a reportes automáticos y comprensibles sobre la calidad y cantidad de agua disponible.

- **Hipótesis 6:**  
  Creemos que se logrará una reducción en los costos operativos del sistema de agua,  
  si los responsables de gestión pueden planificar mantenimientos preventivos usando datos históricos y predicciones del sistema.

- **Hipótesis 7:**  
  Creemos que podremos expandir la adopción de nuestra solución en comunidades rurales diversas,  
  si ofrecemos una plataforma adaptable a distintos niveles tecnológicos y conectividad, gracias al uso de tecnologías como LoRa y GSM.

#### 1.2.2.4. Lean UX Canvas.

A partir de todo lo que hemos investigado, creamos el Lean UX Canvas.


<TABLE BORDER> <TR> <TD ROWSPAN=2><strong>Lean UX Canvas</strong></TD> <TD ROWSPAN=2></TD> <TD></TD> </TR> <TR></TR>


<TR>
  <TD ROWSPAN>
    <strong>1. Business Problem:</strong><br><br>
    En muchas zonas rurales, las comunidades enfrentan un acceso limitado al agua potable debido a una distribución ineficiente y a la falta de información sobre la calidad del agua que consumen. Actualmente, no existen mecanismos efectivos que permitan monitorear en tiempo real tanto la cantidad como la calidad del agua distribuida, lo que impide tomar decisiones informadas para mejorar su distribución y asegurar su salubridad.
  </TD>
  <TD ROWSPAN=2>
    <strong>5. Solutions</strong><br>
    <ul>
      <li><strong>Monitoreo en Tiempo Real:</strong> Uso de sensores IoT para medir caudal, presión, turbidez, niveles de cloro, etc.</li>
      <li><strong>Alertas Automatizadas:</strong> Notificaciones en tiempo real sobre anomalías o interrupciones del servicio.</li>
      <li><strong>Dashboard Centralizado:</strong> Plataforma accesible desde dispositivos móviles o PC para visualizar datos y generar reportes.</li>
      <li><strong>Reportes para la Toma de Decisiones:</strong> Informes periódicos con métricas clave para autoridades y líderes comunitarios.</li>
    </ul>
  </TD>
  <TD ROWSPAN=2>
    <strong>2. Business Outcomes:</strong><br>
    <ul>
      <li>Ser reconocidos como referentes en soluciones IoT para comunidades rurales.</li>
      <li>Reducción del 40% en el tiempo de respuesta ante problemas de suministro.</li>
      <li>Mejora del 25% en estándares de calidad del agua en zonas intervenidas.</li>
      <li>Reducción del 30% en gastos de mantenimiento gracias al análisis predictivo.</li>
      <li>Mayor transparencia y confianza por parte de la comunidad.</li>
    </ul>
  </TD>
</TR>

<TR>
  <TD>
    <strong>3. Users:</strong><br><br>
    <ul>
      <li><strong>Proveedores locales de agua:</strong> Encargados de distribuir, gestionar y mantener el servicio de agua en la comunidad.</li>
      <li><strong>Habitantes de las viviendas:</strong> Personas que consumen el agua y podrían recibir alertas o visualizar información básica (ej. calidad del agua).</li>
    </ul>
  </TD>
</TR>


<TR>
  <TD ROWSPAN=2>
    <strong>6. Hypotheses</strong><br><br>
    <ul>
      <li>Creemos que lograremos reconocimiento como referentes IoT si los usuarios obtienen una experiencia clara con el dashboard.</li>
      <li>Creemos que aumentará la eficiencia si los técnicos reciben alertas en tiempo real.</li>
      <li>Creemos que mejorará la calidad del agua si los parámetros son monitoreados constantemente.</li>
      <li>Creemos que se reducirá el tiempo de respuesta si las alertas llegan al instante a los responsables.</li>
      <li>Creemos que aumentará la confianza comunitaria si se generan reportes automáticos comprensibles.</li>
      <li>Creemos que se reducirán costos operativos si se planifican mantenimientos con base en datos históricos.</li>
    </ul>
  </TD>
  <TD ROWSPAN=2>
  <strong>7. What’s the Most Important Thing We Need to Learn First?</strong><br><br>
  <ul>
    <li>Los usuarios comprenden y valoran el dashboard como una herramienta útil para el monitoreo del agua.</li>
    <li>Las alertas en tiempo real llegan correctamente y son útiles para los técnicos de campo.</li>
    <li>El monitoreo constante de parámetros mejora realmente la calidad del agua distribuida.</li>
    <li>Los reportes automáticos generan confianza en la comunidad al ser claros y comprensibles.</li>
  </ul>
    <TD>
    <strong>4. User Outcomes & Benefits:</strong><br><br>
    <ul>
      <li>Acceso a datos en tiempo real sobre calidad y cantidad del agua.</li>
      <li>Toma de decisiones informadas y rápidas ante emergencias.</li>
      <li>Menor riesgo sanitario mediante acciones preventivas.</li>
      <li>Simplificación de la gestión técnica y operativa.</li>
      <li>Empoderamiento y corresponsabilidad ciudadana en la gestión del agua.</li>
      <li>Mayor confianza entre comunidad y entidades gestoras.</li>
    </ul>
  </TD>
   
</TD>


</TR>

<TR>
  <TD>
    <strong>8. What's the least amount of work we need to do to learn the next most important thing?</strong><br><br>
    <ul>
      <li><strong>Encuestas Rápidas:</strong> A líderes comunitarios y técnicos sobre sus prioridades y retos actuales.</li>
      <li><strong>Pruebas de Concepto:</strong> Implementar un piloto con sensores y dashboard básico en una comunidad.</li>
      <li><strong>Análisis de Factibilidad Técnica:</strong> Validar la cobertura de conectividad en zonas objetivo.</li>
      <li><strong>Recolección de Feedback:</strong> Iterar con base en la experiencia inicial de los usuarios.</li>
    </ul>
  </TD>
</TR>
</TABLE>

## 1.3. Segmentos objetivo.
| Variables    | Segmento 1 - Habitantes | Segmento 2 - Proveedores |
|--------------|-------------------------|---------------------------|
| Geográfica   | Comunidades rurales, asentamientos urbanos marginales o zonas residenciales donde el acceso a agua segura puede ser limitado o de baja calidad. | Empresas de servicios hidráulicos, ONG ambientales o proveedores locales de tecnología situados en zonas rurales, periurbanas o cercanas a zonas de alta necesidad hídrica. |
| Demográfica  | Personas de diversa edad y género, principalmente familias o individuos interesados en mejorar su acceso a agua segura y en cuidar su entorno ambiental. | Profesionales técnicos o comerciales, de edad adulta, con formación o experiencia en gestión de recursos hídricos, instalación de sensores IoT o mantenimiento de redes de agua. |
| Psicológica  | Alta preocupación por la salud, calidad del agua y sostenibilidad. Buscan soluciones simples y accesibles para controlar su propio consumo y asegurar el bienestar familiar. | Enfoque orientado a brindar servicios de alta eficiencia. Valoran la innovación tecnológica para monitorear remotamente sensores, optimizar el uso del agua, cumplir estándares ambientales y ofrecer mantenimiento predictivo. |
