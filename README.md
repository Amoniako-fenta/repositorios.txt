1. Repositorio Frontend: Interfaz de Usuario

Enlace: https://github.com/Amoniako-fenta/mediflow-frontend

Descripción y Propósito: Este repositorio contiene la interfaz de usuario del sistema Mediflow, desarrollada con React y Vite. Su propósito principal es consumir la API del componente BFF para visualizar la información de los pacientes y sus estados de consentimiento. Incluye la implementación de patrones de diseño en la UI (como AlertFactory) y cuenta con una cobertura de pruebas automatizadas superior al 60% utilizando Vitest y React Testing Library, garantizando la estabilidad de los componentes visuales.

2. Repositorio Microservicio BFF: Orquestador (Backend-For-Frontend)

Enlace: https://github.com/Amoniako-fenta/mediflow-bff

Descripción y Propósito: Actúa como el intermediario central y orquestador del ecosistema Mediflow. Desarrollado en Spring Boot (Java 17), su propósito es centralizar las peticiones del frontend y comunicarse de forma segura con los microservicios internos (HCE y Consentimiento) utilizando clientes Spring Cloud OpenFeign. Implementa resiliencia ante caídas de servicios externos y está validado con pruebas unitarias usando Mockito y MockMvc, logrando un 100% de cobertura.

3. Repositorio Microservicio HCE: Historias Clínicas Electrónicas

Enlace: https://github.com/Amoniako-fenta/mediflow-hce-service

Descripción y Propósito: Microservicio core backend encargado de la gestión de pacientes y sus antecedentes médicos (alergias, medicamentos). Desarrollado en Spring Boot, garantiza la persistencia de datos mediante Spring Data JPA utilizando una base de datos relacional H2. Cuenta con endpoints RESTful independientes y un entorno de pruebas de integración completa (Controller-Service-Repository) respaldado por reportes de JaCoCo.

4. Repositorio Microservicio Consentimiento: Gestión de Autorizaciones

Enlace: https://github.com/Amoniako-fenta/mediflow-consent-service

Descripción y Propósito: Microservicio backend independiente dedicado exclusivamente a gestionar y almacenar el estado de autorización (consentimiento) de los pacientes. Al igual que el servicio HCE, asegura la persistencia de los datos en memoria mediante JPA y H2. Su arquitectura aislada permite escalabilidad y está blindada con pruebas de integración que verifican la correcta escritura y lectura en la base de datos (100% de cobertura según JaCoCo).
