# TaL (Tu agente Local)

![Logo TaL](https://github.com/VissanumDev/TaL/blob/main/public/icons/logo_250x121.png)

TaL (Tu agente Local) es una aplicación de escritorio tipo chatbot, ligera, robusta y flexible, construida con **Tauri v2**. Permite interactuar con modelos de IA, tanto locales (con un motor de inferencia propio basado en Rust) como remotos (vía API). Incorpora herramientas "built-in" desarrolladas en Rust, funcionalidades RAG avanzadas sobre documentos locales, gestión de asistentes personalizados y espacios de trabajo.

Diseñada con la privacidad del usuario y el funcionamiento 100% local como prioridades clave, TaL utiliza un backend **Rust** de alto rendimiento y un frontend moderno con **Quasar v2 / Vue v3 / Vite**. La arquitectura está pensada para una posible futura evolución a un modelo cliente-servidor, pero la versión inicial se enfoca en una experiencia de escritorio autocontenida y potente.

## Características Principales

* **Inferencia Local con Rust:** Ejecución de modelos LLM directamente en tu máquina (CPU/GPU) usando un motor optimizado basado en Rust (Candle).
* **Soporte para APIs Externas:** Conexión con proveedores de IA remotos (OpenAI, Anthropic, etc.).
* **RAG Avanzado:** Procesa tus documentos locales para chat contextual. Incluye parseo, chunking, embedding (modelo local), y búsqueda semántica en una base de datos vectorial embebida (LanceDB).
* **Asistentes Personalizados:** Crea y gestiona asistentes con system prompts específicos.
* **Espacios de Trabajo:** Configura entornos aislados para diferentes proyectos o tareas.
* **MCP Client:** Extiende las capacidades de TaL conectándote a servidores de herramientas externos.
* **Herramientas Built-in:** Funcionalidades esenciales integradas en el backend Rust.
* **Experiencia de Escritorio Nativas:** Aprovecha Tauri v2 para una integración profunda con el sistema operativo (Windows, macOS, Linux).
* **Privacidad Prioritaria:** Tus datos permanecen localmente en tu máquina.

## Instalación

* **Usuarios Finales:** Dirígete a la [sección de releases](https://github.com/VissanumDev/TaL/releases) (aún no disponible) para descargar el instalador correspondiente a tu sistema operativo (Windows, macOS, Linux).

* **Desarrolladores:**
    * Consulta la guía de [Configuración del Entorno de Desarrollo](https://github.com/VissanumDev/TaL/blob/main/DEVELOPMENT_ENVIRONMENT.md) para los requisitos y pasos de instalación.
    * Clona el repositorio: `git clone https://github.com/VissanumDev/TaL.git`
    * Sigue las instrucciones en `DEVELOPMENT_ENVIRONMENT.md` para poner en marcha el proyecto.

## Uso

Una vez instalada, inicia la aplicación TaL. La interfaz intuitiva te permitirá:
* Seleccionar modelos de IA locales o remotos.
* Configurar y activar asistentes.
* Gestionar tus documentos para RAG.
* Interactuar en el chat.
* Explorar y conectar servidores MCP.

Consulta la [Documentación para Usuarios](https://github.com/VissanumDev/TaL/tree/main/docs) (aún no disponible) para una guía completa.

## Contribución

¡Nos encantaría tu ayuda para mejorar TaL! Revisa nuestro archivo [Guía de Contribución](https://github.com/VissanumDev/TaL/blob/main/CONTRIBUTING.md) para saber cómo empezar, reportar bugs, sugerir funcionalidades y enviar Pull Requests.

## Stack Tecnológico

* **Framework de Escritorio:** Tauri v2.0
* **Backend:** Rust (Edición 2021) con Tokio
* **Frontend:** Quasar v2 / Vue.js v3 / Vite / TypeScript
* **Inferencia Local:** Candle (Rust)
* **Base de Datos Vectorial (RAG):** LanceDB (Rust)
* **Base de Datos Relacional:** SQL gestionada con SQLx (Rust)
* **Serialización:** Serde (Rust)

## Soporte

Si encuentras algún problema o tienes preguntas, abre un issue en el repositorio de [GitHub Issues](https://github.com/VissanumDev/TaL/issues).

## Licencia

Este proyecto está bajo la Licencia BSD 3-Clause License. Consulta el archivo [LICENSE](https://github.com/VissanumDev/TaL/blob/main/LICENSE) para más detalles.

---
