# 🎥 Proyecto POO en Java: Sistema de Contenido Audiovisual

## 📝 Descripción del Proyecto

Este proyecto implementa los principios fundamentales de la **Programación Orientada a Objetos (POO)** en Java para crear un sistema modular capaz de clasificar, gestionar y mostrar detalles de diferentes tipos de contenido multimedia.

**Propósito:**
* **Demostrar la Herencia y Abstracción:** Utilizando una clase abstracta base (\`ContenidoAudiovisual\`).
* **Implementar Polimorfismo:** A través del método \`mostrarDetalles()\` que se comporta de manera única en cada subclase.
* **Modelar Relaciones:** Aplicando **Agregación** (\`Pelicula\` \-\> \`Actor\`) y **Composición** (\`Documental\` \-\> \`Investigador\`).

***

## 📂 Estructura de Carpetas en GitHub

La estructura de tu proyecto utiliza dos paquetes (`poo` y `uni1a`) dentro de la carpeta fuente (`src`), siendo \`uni1a\` el contenedor de **toda la lógica del sistema**.

Poo_unidad1/
├── .gitignore
├── README.md
└── src/
    ├── poo/
    │   └── PruebaAudioVisual.java (Clase principal de ejecución)
    └── uni1a/
        ├── Actor.java
        ├── ContenidoAudiovisual.java
        ├── Cortometraje.java
        ├── Documental.java
        ├── Investigador.java
        ├── Pelicula.java
        ├── SerieDeTV.java
        ├── Temporada.java
        └── VideoYoutube.java


* **\`src/poo/\`**: Contiene la clase de ejecución que prueba el sistema.
* **\`src/uni1a/\`**: Contiene el 100% de las entidades, subclases, la clase abstracta, y las clases asociadas del sistema.

***

## ✨ Características y Funcionalidades Implementadas

### 1. Clases de Contenido y Entidades Asociadas

| Clase | Concepto POO | Función Principal |
| :--- | :--- | :--- |
| **\`ContenidoAudiovisual\`** | **Clase Abstracta** | Define la estructura básica (\`titulo\`, \`genero\`, \`id\`). |
| **\`Pelicula\`** | Herencia + Agregación | Contiene \`Actor\`es en su \`reparto\`. |
| **\`Documental\`** | Herencia + **Composición** | Depende directamente de un \`Investigador\`. |
| **\`SerieDeTV\`** | Herencia + Agregación | Se compone de múltiples objetos \`Temporada\`. |
| **\`Actor\`**, **\`Temporada\`**, **\`Investigador\`** | Entidades Asociadas | Proporcionan detalles específicos a las clases de contenido. |

### 2. Implementación de POO

* **Encapsulamiento:** Todos los atributos son \`private\` y su acceso es gestionado mediante métodos **Getter y Setter**.
* **Polimorfismo:** El método \`main\` de \`PruebaAudioVisual.java\` itera sobre el array de tipo \`ContenidoAudiovisual\`, y el JVM ejecuta la versión correcta del método \`mostrarDetalles()\` para cada subclase.

***

## 🚀 Instrucciones de Instalación y Uso

### 1. Clonar el Repositorio

Abre tu terminal (o Git Bash) y ejecuta el siguiente comando para descargar el proyecto:

\`\`\`bash
git clone https://github.com/nohemice/Poo_unidad1.git
cd Poo_unidad1
\`\`\`

### 2. Ejecutar la Aplicación Localmente

1.  Abre tu IDE (Eclipse, NetBeans, IntelliJ) e importa el proyecto \`Poo\_unidad1\` como un proyecto Java existente.
2.  Abre la clase principal: **\`PruebaAudioVisual.java\`** (ubicada en \`src/poo/\`).
3.  Ejecuta la clase \`PruebaAudioVisual.java\` haciendo clic en el botón de **Run** (Ejecutar).

La aplicación demostrará la interacción entre los paquetes y la funcionalidad completa del sistema.
