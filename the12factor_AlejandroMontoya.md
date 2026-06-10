# The Twelve-Factor App - Alejandro Montoya

## Factores seleccionados

* Codebase
* Dependencies
* Config
* Dev/Prod Parity

The Twelve-Factor App propone una serie de principios para desarrollar aplicaciones escalables, mantenibles y fáciles de desplegar. Considerando el contexto de Blend360, donde se trabaja con tecnologías en la nube, servicios de AWS, proyectos de datos e inteligencia artificial, considero que los siguientes cuatro factores son los más relevantes debido a su impacto en la colaboración, la reproducibilidad y la confiabilidad de las soluciones.

## ¿Por qué estos cuatro?

### Codebase

En Blend360 se trabaja fuertemente con Git y la colaboración entre equipos. Mantener una única fuente de verdad para cada aplicación facilita el control de versiones, la trazabilidad de los cambios y el trabajo coordinado entre múltiples desarrolladores.

### Dependencies

Los proyectos de datos e inteligencia artificial suelen depender de numerosas librerías y de versiones específicas de estas. Declarar explícitamente las dependencias mediante archivos como `requirements.txt` o `pyproject.toml` permite garantizar la reproducibilidad y asegurar que la aplicación se comporte de manera consistente en diferentes entornos.

### Config

Los proyectos hacen uso de credenciales de AWS, claves de acceso a modelos de IA y otros parámetros de configuración que no deben almacenarse directamente en el código. Separar la configuración de la lógica de la aplicación mediante variables de entorno y servicios de gestión de secretos mejora la seguridad y facilita la administración de diferentes ambientes.

### Dev/Prod Parity

El uso de Docker y otras tecnologías de contenedores permite mantener una alta similitud entre los ambientes de desarrollo y producción. Esto reduce errores durante los despliegues y proporciona mayor confiabilidad al ejecutar aplicaciones, pipelines y servicios relacionados con datos e inteligencia artificial.
