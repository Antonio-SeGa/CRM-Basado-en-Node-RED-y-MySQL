# CRM Basado en Node-RED y MySQL

## Descripción del Proyecto

Este proyecto es un **CRM (Customer Relationship Management)** desarrollado utilizando **Node-RED** y **MySQL**, cuyo objetivo principal es registrar, gestionar, y enviar información relevante a estudiantes de nivel medio superior interesados en la carrera de **Ingeniería en Tecnologías de la Información y Comunicaciones** del ITSOEH.

El CRM se divide en tres módulos principales:

1. **Registro de Estudiantes**: 
   - Un formulario permite registrar los datos de estudiantes interesados, como nombre, apellidos, correo, teléfono, institución educativa y semestre actual.
   - Los datos se almacenan en una base de datos MySQL y se pueden visualizar en una tabla.

2. **Consulta y Actualización de Información**: 
   - El módulo de consulta permite buscar estudiantes previamente registrados utilizando su nombre.
   - Una vez encontrado, se puede actualizar la información de contacto y académica del estudiante.

3. **Envío de Correos Electrónicos**:
   - Se puede enviar correos electrónicos personalizados a los estudiantes filtrando por **institución**. 
   - Se utiliza un formulario para ingresar el asunto y el contenido del correo.
   - El CRM incluye la posibilidad de enviar el correo a todos los estudiantes o a aquellos pertenecientes a una institución específica.

## Resultados

El siguiente apartado muestra los resultados del funcionamiento del CRM, con ejemplos gráficos de la interfaz y de los correos enviados a los estudiantes.

### Ejemplo de Registro de Estudiantes
![Registro de Estudiantes](ruta/a/imagen1.png)

### Ejemplo de Consulta de Información
![Consulta de Información](ruta/a/imagen2.png)

### Ejemplo de Envío de Correo Filtrado por Institución
![Envío de Correo](ruta/a/imagen3.png)

## Flujo de Trabajo en Node-RED

El flujo está compuesto por los siguientes nodos principales:

- **Inyección de datos**: Carga los datos desde la base de datos MySQL.
- **Formulario de Registro**: Permite registrar nuevos estudiantes.
- **Consultas SQL**: Realiza consultas para obtener, actualizar, o insertar datos en la base de datos.
- **Filtros por Institución**: Filtra los estudiantes por la institución ingresada en el formulario.
- **Envío de Correos**: Un módulo dedicado para personalizar y enviar correos electrónicos.

### Visualización del Flujo

Puedes visualizar el flujo de trabajo en Node-RED, que está estructurado en pestañas para cada módulo del CRM:
- **Registro de aspirantes**
- **Consulta de aspirantes**
- **Envío de correo**

## Instalación y Configuración

1. Clona este repositorio.
2. Instala Node-RED y las dependencias necesarias, incluyendo el nodo `node-red-node-mysql`.
3. Configura la conexión a tu base de datos MySQL en el nodo correspondiente.
4. Inicia Node-RED y accede a través del navegador para visualizar el CRM.

### Nota
El archivo de flujo JSON (`flows.json`) está disponible para importar directamente en tu entorno de Node-RED.

## Contacto

Si tienes alguna duda o sugerencia sobre el proyecto, no dudes en contactarme en: `contacto@miempresa.com`.
