# 🐠 Pecera 3D Interactiva - Proyecto de Computación Gráfica

Una aplicación web interactiva que simula una pecera 3D completamente personalizable, desarrollada con **Babylon.js** como proyecto de Computación Gráfica (ESCOM).

## 🎯 Descripción del Proyecto

Este proyecto implementa una escena 3D realista de una **pecera acuática** con múltiples elementos interactivos y efectos visuales avanzados:

### ✨ Características Principales

#### 🎨 **Elementos Visuales**
- **Vidrio transparente** con efectos de especularidad y refracción realista
- **Agua PBR** (Physically Based Rendering) con normal maps animados
- **Algas fractales** generadas proceduralmente usando L-systems (Lindenmayer system)
- **Sistema de partículas** de burbujas con física y contención de límites
- **Pez 3D** importado desde modelo GLB con material Phong
- **Iluminación dinámica** con sol controlable y lámpara interior de la pecera

#### 💡 **Sistemas de Iluminación**
- **Sol direccional**: Controlable en ángulo, intensidad e inclinación
- **Lámpara de la pecera**: SpotLights distribuidos en panel con color y intensidad ajustables
- **Luz hemisférica**: Iluminación ambiental para sombras suaves
- **Environment texture**: Reflejos realistas en superficies

#### 🌿 **Algas Procedurales**
- Generadas con algoritmos L-systems
- **Escalado dinámico** mediante slider interactivo
- Animación de mecido suave (sway animation)
- 10 instancias únicas por pecera con variación aleatoria
- Visibilidad toggleable con checkbox

#### 💧 **Sistema de Agua**
- Material **PBR avanzado** con:
  - Refracción mediante rayos
  - Normal maps animados
  - Transparencia realista
  - Micro-surface y environment intensity ajustables
- Partículas de burbujas:
  - Emisión desde la lámpara
  - Gravedad y dirección controladas
  - Ciclo de vida realista
  - Colisión con límites del agua

### 🎮 **Controles Interactivos**

#### Interfaz gráfica (Panel lateral):
- **Sol**: Control de intensidad, ángulo, inclinación y marcador
- **Lámpara**: Encender/apagar, cambiar color, ajustar intensidad
- **Algas**: Mostrar/ocultar, ajustar tamaño
- **Valores en tiempo real**: Muestra los parámetros actuales

#### Teclado:
- **A/D**: Rotar el sol horizontalmente
- **W/S**: Cambiar inclinación del sol
- **↑/↓**: Ajustar intensidad de la luz solar
- **Rueda del ratón**: Zoom de cámara

#### Cámara:
- **ArcRotate Camera** tipo videojuego
- Zoom suave y fluido
- Rotación con botón derecho

### 🔧 **Tecnologías Utilizadas**

- **Babylon.js**: Motor 3D con WebGL
- **Babylon Loaders**: Carga de modelos GLB
- **Water Material**: Materiales de agua avanzados
- **PBR Materials**: Materiales basados en física
- **L-systems**: Algoritmos para generación procedural de plantas

### 📁 **Estructura del Proyecto**

```
├── index.html          # Aplicación principal
├── pecera1.glb        # Modelo 3D de la pecera base
├── fish.glb           # Modelo 3D del pez
└── README.md          # Este archivo
```

### 🎓 **Conceptos Gráficos Implementados**

1. **Iluminación Phong**: Aplicada en materiales de objetos
2. **Materiales PBR**: Agua con propiedades físicas realistas
3. **Texturas y Normal Maps**: Animación de ondas en el agua
4. **Sistemas de Partículas**: Burbujas con física
5. **L-systems**: Generación procedural de plantas/algas
6. **Culling y Optimización**: Renderizado eficiente
7. **Transparencia y Refracción**: Efectos realistas de vidrio y agua
8. **Sombras y Profundidad**: Pre-pass depth para transparencias

### 🚀 **Cómo Usar**

1. Abre `index.html` en un navegador moderno (Chrome, Firefox, Edge)
2. Usa la **interfaz gráfica** en la esquina superior izquierda para controlar todos los elementos
3. Usa el **teclado** (A, D, W, S, flechas) para controles rápidos del sol
4. **Haz clic y arrastra** con el ratón para rotar la cámara
5. **Rueda del ratón** para hacer zoom

### 📝 **Notas del Desarrollo**

- Try/catch en el callback de Append para manejo robusto de errores
- Checkboxes personalizados con CSS (estilo redondeado y animado)
- Variables de escala base para algas para interpolación suave
- Bounding box calculados dinámicamente para contención de partículas
- Sistema modular con funciones separadas para cada componente (agua, algas, lámpara, etc.)

### 👨‍💻 **Autor**

Proyecto desarrollado por estudiantes de **ESCOM** (Escuela Superior de Cómputo, IPN)
para la materia de **Computación Gráfica**.

---

**Versión**: 1.0  
**Última actualización**: Enero 2026
