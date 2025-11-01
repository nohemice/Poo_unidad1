# 🎥 Proyecto POO en Java: Sistema de Contenido Audiovisual

## 🎯 Objetivos y Propósito del Proyecto

El objetivo principal de este proyecto es aplicar los fundamentos de la **Programación Orientada a Objetos (POO)** en Java para crear un sistema modular y extensible, capaz de clasificar y gestionar varios tipos de contenido multimedia.

**Propósito:**
* **Demostrar la Herencia y el Polimorfismo** utilizando una clase abstracta (\`ContenidoAudiovisual\`) y múltiples subclases.
* **Implementar Relaciones** clave (Agregación y Composición) para modelar dependencias realistas entre entidades (\`Pelicula\` \-\> \`Actor\`).
* **Crear un sistema funcional** y bien documentado que pueda ser fácilmente extendido con nuevos tipos de contenido.

***

## 📂 Estructura de Carpetas en GitHub

El proyecto sigue la estructura estándar para proyectos Java, facilitando la localización y compilación del código fuente.

\`\`\`
Poo_unidad1/
├── src/
│   └── uni1a/
│       ├── Actor.java
│       ├── ContenidoAudiovisual.java
│       ├── Documental.java
│       ├── Pelicula.java
│       ├── PruebaAudioVisual.java
│       ├── ... (todas las clases)
├── .gitignore
└── README.md
\`\`\`

* **\`src/\`**: Carpeta que contiene el código fuente de la aplicación.
* **\`src/uni1a/\`**: Contiene todos los archivos \`.java\` (el código principal del proyecto).

***

## ✨ Clases y Funcionalidades Nuevas Añadidas

Este proyecto implementa múltiples clases y relaciones complejas:

### 1. Clases y Conceptos Clave

| Clase | Concepto POO | Relación Implementada |
| :--- | :--- | :--- |
| **\`ContenidoAudiovisual\`** | Clase **Abstracta** | Base para toda la herencia. |
| **\`Pelicula\`** | Agregación | Relación débil con \`Actor\` ($1 \rightarrow 1..*$). |
| **\`Documental\`** | **Composición** | Relación fuerte con \`Investigador\` ($1 \rightarrow 1$). |
| **\`SerieDeTV\`** | Agregación | Relación débil con \`Temporada\` ($1 \rightarrow 1..*$). |
| **\`Cortometraje\`** / **\`VideoYoutube\`** | Herencia | Nuevas subclases para extender el catálogo. |

### 2. Mejoras Adicionales

* **Encapsulamiento:** Todos los atributos son \`private\` y se gestionan mediante métodos \`public\` **Getter y Setter**.
* **Polimorfismo:** La clase \`PruebaAudioVisual.java\` utiliza el Polimorfismo al iterar sobre el array base (\`ContenidoAudiovisual\`) y llamar a la implementación específica del método \`mostrarDetalles()\` de cada subclase.

***

## 🚀 Instrucciones de Instalación y Uso

### 1. Clonar el Repositorio

Abre tu terminal (o Git Bash) y ejecuta el siguiente comando para descargar el proyecto:

\`\`\`bash
git clone https://github.com/nohemice/Poo_unidad1.git
cd Poo_unidad1
\`\`\`

### 2. Abrir y Ejecutar en Eclipse

1.  Abre **Eclipse IDE**.
2.  Ve a \`File\` \> \`Import...\`.
3.  Selecciona \`General\` \> \`Existing Projects into Workspace\` y haz clic en **Next**.
4.  Haz clic en \`Browse...\` y selecciona la carpeta raíz del proyecto que acabas de clonar.
5.  Asegúrate de que el proyecto \`Poo\_unidad1\` esté seleccionado.
6.  Para ejecutar la aplicación, abre la clase **\`PruebaAudioVisual.java\`** (dentro del paquete \`uni1a\` en la carpeta \`src\`) y haz clic en el botón de **Run** (Ejecutar) para ver la salida en la consola.
