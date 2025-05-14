# Configuración del Entorno de Desarrollo para TaL

Esta guía detalla los requisitos y pasos necesarios para configurar tu máquina local y poder desarrollar la aplicación TaL (Tu agente Local).

## Requisitos del Sistema

* **Sistema Operativo:** Windows (10/11), macOS (Monterey+), o Linux (Ubuntu 20.04+, Fedora 34+, Debian 11+).
* **Espacio en Disco:** Al menos 10 GB libres (los modelos de IA locales y las bases de datos vectoriales pueden ocupar espacio).
* **Memoria RAM:** Mínimo 8 GB, se recomiendan 16 GB o más para modelos de IA más grandes.

## Requisitos de Software

Necesitarás instalar el siguiente software:

1.  **Node.js:** Versión LTS recomendada (actualmente 18.x o 20.x). Incluye npm o yarn. Recomendamos **pnpm** como gestor de paquetes.
    * Instala Node.js: [https://nodejs.org/](https://nodejs.org/)
    * Instala pnpm (si lo prefieres): `npm install -g pnpm`
2.  **Rust:** Instala `rustup` para gestionar las toolchains de Rust. Necesitarás la edición 2021.
    * Sigue las instrucciones en [https://rustup.rs/](https://rustup.rs/)
    * Asegúrate de tener la toolchain estable por defecto: `rustup default stable`
    * Verifica la edición: `cargo --version` (debería ser 1.xx con edición 2021)
3.  **Configuración específica de Tauri v2:** Tauri tiene dependencias específicas del sistema operativo para compilar las aplicaciones nativas.
    * Consulta la documentación oficial de Tauri v2 para tu sistema operativo: [https://tauri.app/v2/guides/prerequisites](https://tauri.app/v2/guides/prerequisites)
    * **Linux:** Necesitarás GCC, pkg-config, WebKit2Gtk development files, etc. Sigue la guía oficial detenidamente.
    * **Windows:** Necesitarás Visual Studio Build Tools con los componentes C++.
    * **macOS:** Necesitarás Command Line Tools for Xcode.
4.  **Editor de Código:** Se recomienda **Visual Studio Code (VSCode)** por su excelente soporte para Rust, Vue, TypeScript y Tauri.
    * Descargar VSCode: [https://code.visualstudio.com/](https://code.visualstudio.com/)
    * Consulta la sección [Configuración Recomendada de VSCode](#configuracion-recomendada-de-vscode) a continuación.
5.  **Git:** Para clonar el repositorio y gestionar versiones.
    * Descargar Git: [https://git-scm.com/downloads](https://git-scm.com/downloads)

## Configuración del Repositorio

1.  **Clona el repositorio de TaL:**
    ```bash
    git clone [https://github.com/VissanumDev/TaL.git](https://github.com/VissanumDev/TaL.git)
    cd TaL
    ```

2.  **Instala las dependencias del Frontend:**
    * Si usas pnpm (recomendado):
        ```bash
        pnpm install
        ```
    * Si usas npm:
        ```bash
        npm install
        ```
    * Si usas yarn:
        ```bash
        yarn install
        ```

3.  **Configura las dependencias de Rust:** Las dependencias del backend se gestionan con Cargo y se descargarán automáticamente cuando compiles el proyecto Rust. No necesitas un paso de instalación separado aquí.

## Configuración Recomendada de VSCode

Para una mejor experiencia de desarrollo en TaL, recomendamos instalar las siguientes extensiones de VSCode:

* **Rust Analyzer:** Soporte avanzado para Rust.
* **Volar (Vue 3, recomendado):** Soporte para archivos `.vue`.
* **ESLint:** Para linting de JavaScript/TypeScript/Vue.
* **Prettier:** Para formato de código (se configurará en la tarea 0.4).
* **EditorConfig:** Para mantener estilos de indentación consistentes.
* **TODO Highlight:** Para resaltar comentarios `TODO`, `FIXME`, etc.

Puedes instalar estas extensiones fácilmente usando el archivo `.vscode/extensions.json` que se encuentra en la raíz del repositorio. Al abrir el proyecto en VSCode, debería aparecer una notificación sugiriendo la instalación de las recomendaciones.

También recomendamos la configuración básica de VSCode proporcionada en el archivo `.vscode/settings.json` para asegurar un formato de código consistente al guardar y otras utilidades de desarrollo.

## Ejecutando el Proyecto

Una vez que tengas todos los requisitos instalados y el repositorio configurado:

1.  Asegúrate de estar en la raíz del repositorio en tu terminal.
2.  Ejecuta el comando de desarrollo de Tauri:
    ```bash
    tauri dev
    ```
    Esto compilará el backend Rust, iniciará el servidor de desarrollo del frontend (Vite) y abrirá la ventana de la aplicación de escritorio TaL. Cualquier cambio en el código (frontend o backend) activará una recarga o recompilación automática.

## Solución de Problemas Comunes

* **Errores de Dependencias de Tauri:** Asegúrate de haber instalado todas las dependencias específicas de Tauri para tu sistema operativo, como se detalla en la documentación oficial de Tauri v2.
* **Problemas de Compilación de Rust:** Ejecuta `cargo check` dentro de la carpeta `src-tauri/` para obtener errores de compilación más detallados. Asegúrate de tener la toolchain Rust correcta instalada (`rustup default stable`).
* **Problemas del Frontend:** Consulta la consola del navegador (puedes abrir las herramientas de desarrollador en la ventana de Tauri) para ver errores de JavaScript/TypeScript.

Si encuentras problemas que no puedes resolver, por favor, abre un Issue en nuestro repositorio de GitHub.

¡Feliz desarrollo con TaL!
