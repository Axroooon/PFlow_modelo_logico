# **PFlow - Modelo Lógico de Base de Datos**



Este directorio contiene el diseño del modelo lógico relacional para PFlow, una solución tecnológica desarrollada por la startup VitalData para optimizar la gestión de flujos, asignación de recursos y tiempos de espera en los departamentos de emergencia hospitalarios.



## **Estructura del Modelo**



El diseño lógico está compuesto por 11 entidades principales normalizadas que resuelven los flujos hospitalarios sin requerir relaciones de muchos a muchos (N:M). El modelo se divide en tres bloques funcionales:



\* Maestros y Catálogos: EstablecimientoSalud, Rol, UsuarioPersonalSalud, AreaAtencion, CamaRecurso.

\* Gestión del Paciente: Paciente, AtencionEmergencia, Triaje.

\* Eventos y Trazabilidad: EventoAtencion, SolicitudServicioApoyo, Interconsulta.



La entidad central para el análisis de datos es EventoAtencion, la cual actúa como bitácora cronológica registrando el historial de uso de camas, tiempos de traslado y atenciones mediante llaves foráneas y marcas de tiempo (DATETIME).



## **Archivos Incluidos**



\* modelo\_logico\_chen.drawio / .png: Diagrama conceptual utilizando notación de Chen para identificar atributos y cardinalidades lógicas.

\* TB1\_BDD-GX.erd: Archivo de diseño relacional lógico-físico.

\* README.md: Documentación de la estructura de datos.



## **Herramientas y Estándares**



\* Entorno de Modelado: Visual Studio Code con la extensión ERD Editor.

\* Notación: Pata de Gallo (Crow's Foot) para el diagrama relacional y notación de Chen para el conceptual.

\* Nomenclatura: Estándar técnico en snake\_case para entidades y atributos.



#### **Instrucciones de Visualización (ERD Editor)**



Para acceder al modelo lógico relacional .erd sin pérdida de codificación:



1\. Abrir la carpeta del proyecto en Visual Studio Code.

2\. Asegurar que la extensión ERD Editor esté instalada y habilitada.

3\. Hacer clic derecho sobre el archivo .erd.

4\. Seleccionar Open With... > ERD Editor para forzar la carga de la interfaz gráfica.

