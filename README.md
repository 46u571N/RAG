# RAG — Guía Visual Interactiva

Una guía educativa completa sobre **Retrieval-Augmented Generation**, construida como una página web estática, interactiva y sin dependencias externas (excepto Google Fonts).

→ **[Ver la guía en vivo](https://tuusuario.github.io/nombre-repo)**

---

## ¿Qué es esto?

Una página web de una sola página (HTML + CSS + JS) que explica RAG de forma visual e interactiva, pensada para equipos técnicos que necesitan entender o comunicar la arquitectura antes de implementarla.

No es una documentación estática. Cada sección tiene widgets interactivos que permiten explorar los conceptos en tiempo real.

---

## Contenido

| Sección | Concepto | Interactividad |
|---|---|---|
| § 01 | El problema que resuelve RAG | Tarjetas informativas |
| § 02 | Pipeline de 5 etapas | Pasos expandibles con detalle |
| § 03 | Embeddings y espacio vectorial | Scatter plot 2D, selección de palabras, líneas de similitud |
| § 04 | Fase de indexación offline | Chunks clicables con vista de registro completo |
| § 05 | Recuperación por similitud coseno | 3 consultas intercambiables, barras animadas |
| § 06 | Estrategias de chunking | 4 tabs con texto resaltado y comparativa de métricas |
| § 07 | Anatomía del registro vectorial | Acordeón con grupos de metadatos |
| § 08 | Construcción del prompt aumentado | Bloques toggle con contador de tokens en tiempo real |
| § 09 | El LLM como redactor | RAG vs LLM estándar, modos de falla |
| § 10 | RAG Moderno (2025–2026) | Hybrid Search, Reranker, Context Compression, Agentic RAG |

---

## Uso

Es un solo archivo HTML. Sin build, sin dependencias locales, sin framework.

```bash
# Clonar
git clone https://github.com/tuusuario/nombre-repo.git

# Abrir directo en el browser
open index.html
```

Para verlo en un servidor local:

```bash
# Python 3
python -m http.server 8000

# Node
npx serve .
```

---

## Deploy en GitHub Pages

1. Asegurate de que el archivo se llame `index.html`
2. En el repo: **Settings → Pages → Branch: main → / (root) → Save**
3. La URL queda disponible en `https://tuusuario.github.io/nombre-repo` en ~60 segundos

---

## Stack técnico

- HTML5 + CSS3 + Vanilla JS — sin frameworks
- Google Fonts: DM Sans + DM Mono
- SVG para visualización de embeddings (generado dinámicamente por JS)
- Sin dependencias npm, sin build step, sin cookies, sin tracking

---

## Contexto

Esta guía fue creada como material de referencia para equipos que están evaluando o implementando arquitecturas RAG sobre bases de conocimiento privadas (registros clínicos, documentación interna, bases de datos corporativas).

Cubre tanto el RAG clásico de 5 pasos como las técnicas de producción actuales:

- **Hybrid Search** — BM25 + búsqueda semántica (Reciprocal Rank Fusion)
- **Reranker** — Cross-Encoder para re-puntuar candidatos
- **Context Compression** — Reducción de tokens antes del prompt
- **Agentic RAG** — El LLM decide cómo y cuándo recuperar

---

## Licencia

MIT — libre para usar, modificar y distribuir.
