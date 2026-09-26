# rascal-mono 🚀

**rascal-mono** es una extensión de alto rendimiento para el lenguaje de metaprogramación **Rascal**, diseñada para proporcionar análisis estático de código, transformación de programas y reingeniería sobre la plataforma de código abierto **Mono / .NET (ECMA CLI)** y el ecosistema C#.

Desarrollada para integrarse con la infraestructura de ejecución de Rascal, esta extensión permite a los investigadores y desarrolladores analizar sintáctica y semánticamente proyectos C#, inspeccionar ensamblados CIL/CLI de .NET y realizar transformaciones de código fuente a gran escala de forma rápida y estructurada.

---

## 🌟 Características Principales

* **Análisis Sintáctico y Semántico de C#:** Extracción de Árboles de Sintaxis Abstracta (AST) y grafos de flujo de control (CFG) para proyectos C# basados en especificaciones ECMA.
* **Inspección de Ensamblados CIL/CLI (.NET):** Mapeo de metadatos de archivos `.dll` y `.exe` compilados para la plataforma Mono/.NET hacia tipos de datos algebraicos de Rascal.
* **Transformación y Refactorización de Código:** Aplicación de reglas de reescritura de términos (*term rewriting*) para la automatización de migraciones de código de C# y modernización de sistemas .NET.
* **Integración con la Cadena de Herramientas Rascal:** Compatibilidad total con las primitivas de análisis de relaciones, gramáticas concretas e instrumentos de análisis estático nativos de Rascal.

---

## 🏗️ Arquitectura de la Plataforma

* **Rascal C# / CLI Extractor:** Herramienta encargada de procesar código fuente C# y binarios CIL/ECMA-335 para convertirlos en representaciones M3/AST dentro del entorno de Rascal.
* **Mono Meta-Model Bridge:** Capa de abstracción que mapea la jerarquía de tipos de la Base Class Library (BCL) y elementos del Common Language Runtime hacia relaciones de Rascal.
* **Transformation Engine:** Motor de reescritura que ejecuta transformaciones de código C# garantizando la preservación de la semántica del lenguaje.

---

## 🚦 Inicio Rápido

### Prerrequisitos

* **Rascal CLI / Eclipse Rascal Plugin** (instalación activa de Rascal).
* **Mono Runtime / .NET SDK** instalado y disponible en el sistema.

### Instalación

```bash
# Clonar el repositorio
git clone [https://github.com/tu-usuario/rascal-mono.git](https://github.com/tu-usuario/rascal-mono.git)
cd rascal-mono

# Compilar los módulos de extracción e integración
rascal-shell pack
