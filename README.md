# 📘 TACA-ENV – Libro/Web de Teoría de Autómatas

Este repositorio contiene un proyecto desarrollado con **Quarto** para crear un
**libro de recopilación de Teoría de Autómatas** que se publica tanto como:

- 🌐 **Sitio web / libro web** (HTML navegable).
- 📕 **Libro descargable** (PDF).
- 🧾 (Opcional) **Fuente LaTeX consolidada**.

El objetivo es ofrecer un recurso didáctico estructurado para estudiantes de
Teoría de Autómatas y Lenguajes Formales, conectando la **base teórica** con
**ejemplos y aplicaciones en informática y desarrollo de software**.

---
## 🛠 Tecnologías utilizadas

**Quarto**
 – motor de publicación científica/técnica.
**R**
 + paquetes knitr y rmarkdown (para la
ejecución de documentos Quarto).
(Opcional) TinyTeX – para la generación de PDF a partir del proyecto.
GitHub Actions – para integración continua (CI).

## 🚀 Cómo trabajar con el proyecto en local
1. Requisitos previos: En tu máquina local necesitas tener instalado:
Quarto.
R (si usas chunks de R o PDF).
Paquetes de R recomendados:
install.packages(c("knitr", "rmarkdown"))
(Opcional) TinyTeX, si quieres generar PDF localmente:

install.packages("tinytex")
tinytex::install_tinytex()

2. Clonar el repositorio
git clone https://github.com/<usuario>/<nombre-repo>.git
cd <nombre-repo>/taca-env

3. Verificar el proyecto Quarto
quarto check


Si todo está correcto, verás un resumen de la configuración sin errores.
4. Renderizar el libro como sitio web (HTML)
quarto render --to html
Esto generará la salida (por defecto) en la carpeta _book/ dentro de taca-env/.
5. Renderizar el libro como PDF
quarto render --to pdf
Se generará un PDF consolidado del libro (puede tardar más que la versión HTML).
6. Previsualizar como servidor local
quarto preview
Abre el navegador con una vista dinámica del libro; los cambios en los .qmd
se reflejan automáticamente.

## ✉️ Contacto

Para comentarios, sugerencias o reportes de errores:

Abre un Issue en la pestaña Issues del repositorio, o Escribe a: **crisitan.narvaez@unl.edu.ec**

---

## 📂 Estructura del repositorio

```text
.
├── taca-env/                 # Proyecto Quarto del libro
│   ├── _quarto.yml           # Configuración principal del libro
│   ├── index.qmd             # Portada / página principal
│   ├── preface.qmd           # Prefacio
│   ├── introduccion.qmd      # Introducción
│   ├── participantes.qmd     # Sección de participantes del libro
│   ├── ...                   # Capítulos (01-*, 02-*, etc.)
│   └── assets/               # Recursos (PDF, LaTeX, imágenes, etc.)
└── .github/
    └── workflows/
        └── quarto-ci.yml     # Workflow de CI para validar y renderizar el libro

