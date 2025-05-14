# Guía para Contribuir a TaL

¡Gracias por considerar contribuir a TaL! Tu ayuda es muy valiosa para mejorar esta aplicación. Este documento detalla el proceso para que tu contribución sea lo más fluida posible.

## Código de Conducta

Este proyecto se rige por un Código de Conducta. Al participar, se espera que respetes este código. [Incluir enlace a CODE_OF_CONDUCT.md si existe, o detallarlo aquí].

## ¿Cómo puedo contribuir?

Hay muchas formas de contribuir a TaL:

1.  **Reportar Bugs:** Si encuentras un error, por favor, abre un Issue en GitHub describiendo el problema con el mayor detalle posible.
2.  **Sugerir Funcionalidades:** ¿Tienes una idea para mejorar TaL? Abre un Issue para discutirla.
3.  **Escribir Código:** Implementa nuevas funcionalidades o corrige bugs.
4.  **Mejorar la Documentación:** Ayuda a que nuestra documentación sea clara y completa.
5.  **Revisar Código:** Revisa Pull Requests de otros colaboradores.

## Reportando Bugs

Antes de reportar un bug, busca en los Issues existentes para ver si ya ha sido reportado. Si no, abre un nuevo Issue y proporciona la siguiente información:

* **Descripción Clara:** Explica el problema y el comportamiento esperado.
* **Pasos para Reproducir:** Describe cómo podemos reproducir el bug. Sé lo más preciso posible.
* **Entorno:** Indica tu sistema operativo, versión de TaL, y cualquier otra información relevante sobre tu entorno (versión de Rust, Node.js, etc.).
* **Capturas de Pantalla o Videos:** Si es posible, adjunta imágenes o un video que muestre el bug.
* **Logs:** Incluye cualquier mensaje de error de la consola de desarrollo (Frontend) o de la terminal donde ejecutaste `tauri dev` (Backend Rust).

## Sugiriendo Funcionalidades

Abre un Issue en GitHub y describe la funcionalidad que te gustaría añadir o modificar. Explica por qué crees que sería útil para TaL y, si tienes ideas, cómo podría implementarse. Esto nos permite discutir la idea antes de que inviertas tiempo en desarrollarla.

## Contribuyendo con Código o Documentación

Sigue estos pasos para enviar tu código o documentación:

### 1. Configura tu Entorno de Desarrollo

Consulta el archivo [`DEVELOPMENT_ENVIRONMENT.md`](https://github.com/VissanumDev/TaL/blob/main/DEVELOPMENT_ENVIRONMENT.md) para obtener instrucciones detalladas sobre cómo configurar tu entorno con Rust, Node.js, Quasar/Vue, Tauri y VSCode.

### 2. Flujo de Trabajo Git

Utilizamos un flujo de trabajo basado en ramas (Git Flow simplificado).

* **Rama Principal (`main`):** Contiene la última versión estable y liberada.
* **Rama de Desarrollo (`develop`):** Es la rama de integración principal para las funcionalidades en curso. Las ramas de trabajo se crean a partir de `develop`.
* **Ramas de Trabajo:** Crea una rama específica para cada tarea (funcionalidad, bugfix, tarea de mantenimiento) partiendo siempre de `develop`.

    * **Convención de Nombre:** Utiliza un prefijo seguido de una barra, un área/componente y una descripción breve en kebab-case.
        * `feature/<area>-<descripcion>` (ej: `feature/RUST-servicio_inferencia_candle`)
        * `fix/<area>-<descripcion>` (ej: `fix/RAG-error_busqueda_vacia`)
        * `chore/<area>-<descripcion>` (ej: `chore/DEPS-actualizar_tokio`)
        * `<area>` puede ser: `UI`, `RUST`, `RAG`, `DOCS`, `CI`, `DEPS`, `BUILD`, `MCP`, `TOOL`, `CORE`, etc.

* **Proceso:**
    1.  Asegúrate de estar en la rama `develop` local y que esté actualizada:
        ```bash
        git checkout develop
        git pull origin develop
        ```
    2.  Crea tu nueva rama de trabajo:
        ```bash
        git checkout -b <nombre_de_tu_rama> # Siguiendo la convención
        ```
    3.  Realiza tus cambios, haciendo **commits atómicos y descriptivos** frecuentemente. Utiliza la [Convención de Mensajes de Commit](#convencion-de-mensajes-de-commit).
    4.  Sube tu rama de trabajo a GitHub regularmente:
        ```bash
        git push -u origin <nombre_de_tu_rama>
        ```
    5.  Una vez que tu trabajo esté completo y probado localmente:
        * Asegúrate de que tu rama `develop` local está actualizada: `git checkout develop && git pull origin develop`.
        * Vuelve a tu rama de trabajo y haz un `git merge develop` para incorporar los últimos cambios (resuelve conflictos si los hay).
        * Sube los cambios de tu rama de trabajo actualizados: `git push origin <nombre_de_tu_rama>`.
        * Abre un **Pull Request (PR)** en GitHub desde tu rama de trabajo hacia la rama `develop`.

### 3. Convención de Mensajes de Commit

Utilizamos una convención de mensajes de commit sencilla pero descriptiva. Cada mensaje debe tener la siguiente estructura:

* **`tipo`:** Indica la naturaleza del cambio. Ejemplos:
    * `feat`: Nueva funcionalidad.
    * `fix`: Corrección de un bug.
    * `docs`: Cambios en la documentación.
    * `style`: Cambios que no afectan el significado del código (espacios en blanco, formato, puntos y comas, etc.).
    * `refactor`: Un cambio de código que no corrige un bug ni añade una funcionalidad.
    * `perf`: Cambio de código que mejora el rendimiento.
    * `test`: Añadir o modificar pruebas.
    * `chore`: Tareas de mantenimiento o cambios en herramientas/configuración (gitignore, dependencias, etc.).
    * `build`: Cambios que afectan el sistema de build o dependencias externas.
    * `ci`: Cambios en los archivos y scripts de CI.
* **`(área)` (Opcional pero recomendado):** Indica el componente o área afectada por el cambio (ej: `(RUST)`, `(UI)`, `(RAG)`, `(CI)`).
* **`descripción breve`:** Un resumen conciso del cambio (máx. 50 caracteres), comenzando con mayúscula y en imperativo (ej: "Añadir soporte...", "Corregir cálculo...").
* **Cuerpo del mensaje (Opcional):** Proporciona detalles adicionales sobre el cambio. Cada línea no debe superar los 72 caracteres.

**Ejemplos:**

feat(RUST): Implementar servicio de inferencia local con Candle
Añade la estructura inicial del servicio de inferencia en Rust
utilizando el crate Candle. Permite cargar modelos GGUF
y realizar inferencias básicas.

fix(UI): Corregir visualización de mensajes largos en el chat
Ajusta el estilo CSS para asegurar que los mensajes del chat
con contenido extenso no desborden el contenedor y permitan scroll.

chore(gitignore): Actualizar reglas para incluir archivos de build de Tauri

### 4. Pull Requests

Abre tu Pull Request (PR) lo antes posible (incluso si el trabajo no está terminado - marca el PR como "Draft"). Esto permite que otros vean tu progreso y proporcionen feedback temprano.

* **Título del PR:** Usa una convención similar a los mensajes de commit (`tipo(área): descripción`).
* **Descripción del PR:**
    * Describe el problema que resuelve o la funcionalidad que implementa.
    * Haz referencia al Issue relacionado (ej: `Fixes #123`, `Implements #456`).
    * Incluye una lista de los cambios realizados.
    * Explica cómo probaste tus cambios.
    * Si el PR no está listo, indícalo claramente (ej: "WIP - Work In Progress").
* **Revisión:** Solicita la revisión de al menos un mantenedor del repositorio. Aborda los comentarios y sugerencias recibidas.

### 5. Estándares de Código

* **Rust:** Seguir las convenciones de `rustfmt` y las recomendaciones de `clippy` (con un nivel de exigencia alto). Utilizar las características idiomáticas del lenguaje.
* **TypeScript/Vue:** Seguir las convenciones definidas en la configuración de ESLint y Prettier (se configurará en la tarea 0.4). Usar TypeScript de forma estricta y tipar correctamente el código.
* **General:** Mantener el código legible, modular y bien documentado.

### 6. Pruebas

* Se espera que las contribuciones incluyan pruebas:
    * **Rust:** Pruebas unitarias (`#[test]`), pruebas de integración.
    * **TypeScript/Vue:** Pruebas unitarias de componentes y lógica (con Vitest u otra herramienta).
* Asegúrate de que todas las pruebas existentes pasen.

Al seguir estas pautas, ayudas a mantener la calidad y coherencia del proyecto TaL. ¡Gracias de nuevo por tu contribución!
