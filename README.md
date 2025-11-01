# 🎥 Proyecto POO en Java: Sistema de Contenido Audiovisual

## 🎯 Objetivos y Propósito del Proyecto

El objetivo principal de este proyecto es aplicar los fundamentos de la **Programación Orientada a Objetos (POO)** en Java para crear un sistema modular y extensible, capaz de clasificar y gestionar varios tipos de contenido multimedia.

**Propósito:**
* **Demostrar la Herencia y el Polimorfismo** utilizando una clase abstracta (\`ContenidoAudiovisual\`) y múltiples subclases.
* **Implementar Relaciones** clave (Agregación y Composición) para modelar dependencias realistas entre entidades (\`Pelicula\` \-\> \`Actor\`).
* **Crear un sistema funcional** y bien documentado que pueda ser fácilmente extendido con nuevos tipos de contenido.

***

## ✨ Clases y Funcionalidades Nuevas Añadidas

Este proyecto se expandió significativamente desde su diseño inicial, añadiendo nuevas entidades y perfeccionando las relaciones.

### 1. Clases Añadidas

| Clase | Función | Relación Implementada |
| :--- | :--- | :--- |
| **\`Actor\`** | Entidad de soporte para las películas. | **Agregación** con \`Pelicula\` ($1 \rightarrow 1..*$). |
| **\`Temporada\`** | Entidad que estructura las series de televisión. | **Agregación** con \`SerieDeTV\` ($1 \rightarrow 1..*$). |
| **\`Investigador\`** | Entidad asociada al autor principal de un documental. | **Composición** con \`Documental\` ($1 \rightarrow 1$). |
| **\`Cortometraje\`** | Nueva subclase de \`ContenidoAudiovisual\` con atributos (\`festival\`, \`anioEstreno\`). | **Herencia**. |
| **\`VideoYoutube\`** | Nueva subclase de \`ContenidoAudiovisual\` con atributos de plataforma (\`canal\`, \`visualizaciones\`). | **Herencia**. |

### 2. Mejoras Adicionales e Implementación

* **Encapsulamiento Completo:** Todos los atributos son \`private\` y se accede a ellos únicamente a través de métodos \`public\` **Getter y Setter**.
* **Polimorfismo en el Bucle:** La clase \`PruebaAudioVisual.java\` utiliza un bucle \`for\` sobre el *array* de tipo \`ContenidoAudiovisual\`, llamando al método \`mostrarDetalles()\` de cada objeto, garantizando que se ejecute el código de la subclase correcta.
* **Uso de Colecciones:** Se utiliza \`List<T>\` (implementado con \`ArrayList\`) para manejar las relaciones de Agregación, como el \`reparto\` de una \`Pelicula\` y las \`temporadas\` de una \`SerieDeTV\`, haciendo el código más flexible.

***

## 🚀 Instrucciones para Clonar y Ejecutar

Sigue estos pasos para obtener y ejecutar el proyecto en tu máquina local.

### 1. Clonar el Repositorio

Abre tu terminal (o Git Bash) y ejecuta el siguiente comando:

\`\`\`bash
git clone https://github.com/TU_USUARIO/Sistema-Contenido-Audiovisual-POO.git
cd Sistema-Contenido-Audiovisual-POO
\`\`\`

### 2. Abrir y Ejecutar en Eclipse

1.  Abre **Eclipse IDE**.
2.  Ve a \`File\` \> \`Import...\`.
3.  Selecciona \`General\` \> \`Existing Projects into Workspace\`.
4.  Haz clic en \`Browse...\` y selecciona la carpeta raíz del proyecto que acabas de clonar.
5.  Para ejecutar, abre \`PruebaAudioVisual.java\` (dentro del paquete \`uni1a\`) y haz clic en el botón de **Run** (Ejecutar).
