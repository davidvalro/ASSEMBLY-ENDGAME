# 💻 Assembly: Endgame

Un proyecto moderno del juego clásico del Ahorcado, construido con **React, TypeScript y Vite**, pero con un giro de alto rendimiento: la lógica central del juego se reescribe en **AssemblyScript** y se compila a **WebAssembly (WASM)** para lograr una velocidad cercana a la nativa en el navegador.

El juego está temáticamente centrado en el mundo de la programación: tienes un número limitado de "lenguajes de programación" (tus vidas) para adivinar la palabra antes de que `Assembly` (WebAssembly) tome el control de todo.

### 🚀 Tecnologías Principales

| Tecnología | Rol |
| :--- | :--- |
| **React** | Framework para construir la interfaz de usuario (UI) y gestionar el estado del juego. |
| **TypeScript (TSX)** | Usado en la capa de React para mayor seguridad de tipos y mejor desarrollo. |
| **Vite** | Herramienta de construcción (bundler) moderna y rápida. |

### 🛠️ Estructura del Proyecto

La estructura del proyecto refleja la división de responsabilidades entre el *frontend* (React) y el motor de rendimiento (AssemblyScript):