# Release Notes — v1.0.0 (2025-10-17)

## 📦 Resumen
**Lista etiquetas atributos eventos XSS** concentra en un solo lugar **todas** las superficies HTML/SVG/MathML (etiquetas, atributos y eventos) para **fuzzing, payload generation y bypasses**. Ahorra horas de investigación y reduce omisiones críticas.

---

## 🧪 Problema que resuelve
La información de etiquetas/atributos/eventos está dispersa entre estándares, wikis y documentación oficial. Eso provoca:
- Vectores ignorados por falta de catálogo práctico.
- Pérdida de tiempo al construir diccionarios y wordlists.
- Menor creatividad para mutaciones y cadenas XSS.

---

## ⚙️ Qué aporta y cómo beneficia
- **Cobertura total**: HTML, SVG, MathML (incluye obsoletos/experimentales útiles).
- **Velocidad**: listas listas para copiar en fuzzers/generadores de payloads.
- **Creatividad**: inspira combinaciones raras para romper filtros y WAFs.
- **Estandarización**: una única fuente para tu arsenal ofensivo.

---

## 🗂️ Contenido (extracto)
- **Etiquetas HTML**: `html, head, title, base, link, meta, style, script, noscript, template, slot, body, header, footer, main, nav, section, article, aside, h1–h6, p, br, hr, pre, blockquote, cite, q, abbr, dfn, address, time, mark, small, strong, em, b, i, u, s, del, ins, sub, sup, code, kbd, samp, var, div, span, ul, ol, li, dl, dt, dd, figure, figcaption, img, picture, source, canvas, svg, path, circle, …, iframe, object, embed, audio, video, track, form, input, button, select, textarea, …, table, thead, tbody, tfoot, tr, th, td, details, summary, dialog, menu, …, data, bdi, bdo, wbr, ruby, rt, rp, obsoletos (marquee, font, center, applet, frame…), experimentales (module, modulepreload)`  
- **MathML**: `math, mrow, mfrac, msqrt, mtext, mo, mi, mn, …`
- **SVG**: `svg, script, foreignObject, image, path, animate*, filter*, fe*, use, …`
- **Atributos**: globales (`id, class, style, title, hidden, tabindex, contenteditable, dir, lang, …`), enlaces (`href, target, rel, referrerpolicy…`), recursos (`src, crossorigin, integrity, …`), formularios/inputs, `iframe`, `script`, `link`, `meta`, **ARIA**, **experimentales** (`popover, inert, blocking, enterkeyhint, …`), **SVG** (`fill, stroke, d, transform, viewBox, …`), **MathML** (`mathvariant, mathsize, …`) y **obsoletos**.
- **Eventos**: ratón/puntero (`onclick, onpointerdown, …`), teclado, foco, formularios, carga/recursos (`onload, onerror`), UI global (`onresize, onscroll…`), drag&drop, multimedia, portapapeles, animaciones/transiciones, sensores, gamepad, speech, notificaciones/push, WebRTC, Bluetooth/USB/Serial, WebXR, pagos.

> **Nota**: el repos incluye las listas completas (ver archivo fuente).

---

## 🧠 Uso recomendado
1. **Fuzzing**: genera diccionarios por contexto (etiqueta/atributo/evento) y combínalos.
2. **Payload factory**: cruza etiquetas raras + atributos poco usados + eventos exóticos.
3. **Bypass WAF**: mezcla obsoletos/experimentales que algunos parsers aceptan laxo.
4. **Auditoría**: chequea **what-if** por contexto (HTML inline, SVG, MathML, srcdoc, etc.).

---

## 🛣️ Roadmap
- ✅ v1: Catálogo estático completo.
- ⏭️ v1.1: Export JSON/CSV listos para fuzzers.
- ⏭️ v1.2: Marcado de “compatibilidad/soporte” y “riesgo XSS” por ítem.

---

**Tu diccionario maestro de superficie HTML para XSS avanzado.**
