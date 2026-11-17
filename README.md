# ComidApp · Módulo de Recetas con IA

Repositorio de presentación del módulo de recetas de **ComidApp**, un proyecto de equipo realizado en el Instituto Politécnico Modelo. El código fuente vive en un repositorio privado de la organización; acá se resume qué hace y cómo está armado.

## Qué es

Un servicio en **Python 3.12 + FastAPI** que ofrece tres capacidades al resto del sistema:

- **Búsqueda** de recetas.
- **Generación** de recetas con un modelo de lenguaje (LLM).
- **Sincronización** del catálogo de recetas.

El módulo es consumido por la API principal del sistema, escrita en Java.

## Tecnologías

- Python 3.12 y FastAPI
- LLM para la generación de recetas
- Qdrant (base de datos vectorial) para la búsqueda
- Redis
- RabbitMQ para la mensajería entre servicios
- Docker y Docker Compose para la infraestructura local

## Características

- Carga de datos iniciales cuando la colección está vacía.
- Validación de credenciales del LLM al iniciar el servicio.
- Tareas periódicas de reconciliación y de regeneración del catálogo.
- Documentación por endpoint y guías de despliegue (desarrollo y producción).
- Desarrollo guiado por especificaciones (spec-driven): una especificación por cada funcionalidad.

## Equipo

Proyecto de equipo del Instituto Politécnico Modelo.
