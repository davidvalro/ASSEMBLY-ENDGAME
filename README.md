# 💻 Assembly: Endgame: El Ahorcado de Alto Rendimiento

## 🚀 Juego de Adivinanza con React, TypeScript y WASM (WebAssembly)

### 📝 Descripción del Proyecto

**Assembly: Endgame** es una aplicación web que revoluciona el clásico juego del Ahorcado. Este proyecto es una demostración de arquitectura moderna al combinar un frontend avanzado con un motor de alto rendimiento.

El juego está construido con **React y TypeScript**, y la lógica central del juego se diseña para ser eficiente, con referencias a posibles implementaciones reescritas en **AssemblyScript** y compiladas a **WebAssembly (WASM)**. Esto simula cómo se podría ejecutar la lógica crítica (como el chequeo de intentos o la actualización del estado) con una **velocidad cercana a la nativa** directamente en el navegador.

El juego está temáticamente centrado en el mundo de la programación: tienes un número limitado de "lenguajes de programación" (tus vidas) para adivinar la palabra antes de que `Assembly` tome el control.

---

### 🌟 Arquitectura y Funcionalidades Clave

Este proyecto utiliza un patrón de diseño que separa claramente la **Presentación** de la **Lógica del Juego**, usando TypeScript para una mayor seguridad.

| Módulo | Responsabilidad | Tecnología Principal |
| :--- | :--- | :--- |
| **Frontend (UI)** | Renderizado de componentes, manejo de eventos del usuario (teclado), efectos visuales y orquestación del estado general del juego. | **React + TypeScript (TSX)** |
| **Motor de Lógica** | Lógica de cálculo crítico del juego (manejo de vidas, verificación de aciertos) y gestión de estados derivados. | **TypeScript / WebAssembly (WASM)** |

#### Características Frontend Destacadas

| Característica | Detalle Técnico | Archivos Clave |
| :--- | :--- | :--- |
| **Tipado Fuerte** | Uso riguroso de **TypeScript** en toda la capa de React para garantizar la seguridad de tipos, interfaces claras y mejor escalabilidad. | `tsconfig.*.json` |
| **Estados Derivados** | Cálculo eficiente de propiedades reactivas como `isGameWon`, `isGameLost` y `wrongGuessCount` a partir de estados base, eliminando la redundancia. | `App.jsx` |
| **UX Dinámico** | Uso de efectos visuales (`react-confetti`) al ganar y manejo de clases dinámicas (`clsx`) para retroalimentación visual en el teclado. | `package.json` |
| **Accesibilidad (A11y)** | Implementación de regiones **`aria-live`** para anunciar el estado del juego y los resultados de las adivinanzas a lectores de pantalla. | `App.jsx` |

---

### 💻 Stack Tecnológico

El proyecto está construido sobre el ecosistema moderno de desarrollo web:

* **Framework Principal:** React
* **Lenguaje Base:** TypeScript (TSX)
* **Motor de Rendimiento (Concepto):** WebAssembly (WASM)
* **Gestión de Clases:** `clsx`
* **Bundler/Servidor:** Vite
* **Herramientas de Desarrollo:** ESLint, TypeScript Compiler

---

### 🚀 Cómo Empezar (Guía de Ejecución Local)

Para clonar y ejecutar el proyecto en tu máquina:

1.  **Instala las dependencias necesarias** (incluyendo las dependencias de TypeScript):
    ```bash
    npm install
    ```
2.  **Inicia la aplicación** en el servidor de desarrollo local:
    ```bash
    npm run dev
    # o npm start
    ```

---

### 👨‍💻 Nota del Desarrollador

Este proyecto fue concebido como un estudio de caso en **arquitectura de aplicaciones web modernas**. Su principal objetivo es demostrar la integración efectiva de una capa de lógica de alto rendimiento (simulando **WebAssembly - WASM**) dentro de un *stack* React/TypeScript.

La justificación de este enfoque se centra en la **separación de preocupaciones**: se delegan los procesos computacionalmente intensivos a un módulo optimizado (WASM) mientras que React se encarga de la flexibilidad, el manejo de estados de la UI y el desarrollo rápido de la interfaz.

El uso de **TypeScript** en el *frontend* complementa esta arquitectura, garantizando un código más robusto, mantenible y escalable gracias al **tipado estático** y a la definición clara de interfaces.
