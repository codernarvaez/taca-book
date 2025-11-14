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
