🌌 Catálogo Cósmico Hiperbólico: Visualización del Universo con d3-hypertree

https://marielnr.github.io/Hyperbolic-Tree-Messier-Hipparcos-/

Este proyecto implementa una **Visualización de Árbol Hiperbólico** interactiva para explorar datos astronómicos (como el Catálogo Messier) utilizando la librería JavaScript `d3-hypertree`.

La librería utiliza **geometría hiperbólica** para mapear una jerarquía densa de datos en un espacio 2D (el Disco de Poincaré), permitiendo una exploración detallada sin la sensación de hacinamiento que se da en los gráficos de árbol planos.

---

## ✨ Características Principales

* **Geometría No-Euclídea:** Mapea la jerarquía de datos (`Raíz` → `Constelación` → `Objeto Cósmico`) en un **Disco de Poincaré** para una visualización eficiente.
* **Interacción Inmersiva:** La vista se expande suavemente hacia el centro al seleccionar un nodo, ofreciendo una experiencia de navegación sin perder el contexto global.
* **Metadatos Visuales:** Se utiliza un *emojimap* dinámico para asignar **íconos emoji** representativos a las constelaciones (ej. *Hércules* 💪, *León* 🦁), enriqueciendo la experiencia visual.
* **Carga Nativa:** Utiliza el método nativo de carga de archivos (`hyt.loaders.fromFile`) para inyectar el JSON directamente, asegurando la máxima compatibilidad con esta versión de la librería.

---

## 🛠️ Tecnologías y Archivos Clave

El proyecto está diseñado para funcionar con un conjunto de archivos **minimalista y autocontenido**, reflejando la estructura original de los ejemplos.

| Archivo | Función |
| :--- | :--- |
| **`index.html`** | Estructura principal, contiene el *script* de inicialización del `Hypertree`. |
| **`d3-hypertree.js`** | La librería de visualización (debe ser una versión estable). |
| **`d3-hypertree-light.css`** | Estilos CSS para el aspecto del disco, los nodos y las etiquetas. |
| **`hyperbolic_tree_data_simple.json`** | **Datos de entrada:** Catálogo astronómico en formato de objeto raíz jerárquico. |
| **`labels.json`** | Archivo de etiquetas opcional para el `langloader`. |

---

## 🚀 Instalación y Ejecución

Simplemente clona el repositorio y abre el archivo `index.html`.

### Requisitos

Solo se necesita un navegador moderno. **No requiere** la instalación de Node.js, npm, o librerías D3 externas, ya que `d3-hypertree.js` es un *bundle* autocontenido.
