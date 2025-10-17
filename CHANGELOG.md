# Changelog

Todas las versiones siguen [SemVer].

## [v1.0.0] - 2025-10-17
### 🆕 Añadido
- **Lista etiquetas atributos eventos XSS**: base ofensiva con **HTML/SVG/MathML** (etiquetas), **atributos** (globales, específicos, obsoletos, experimentales) y **eventos** (UI/teclado/multimedia/sensores/…).
- **Propósito**: fuzzing, generación de payloads, diccionarios personalizados y bypasses de WAF.
- **Bloques incluidos**:
  - Listado extenso de **etiquetas HTML** (head/metadata, body/secciones, inline, figuras, multimedia, formularios, tablas, interactivos, varios, obsoletos y experimentales).
  - **MathML** y **SVG** con elementos relevantes para vectores XSS.
  - **Atributos**: globales, contenido, enlaces, media, formularios, inputs, botones, tablas, imágenes/mapas, iframe, script, link, meta, ARIA, experimentales, SVG, MathML y obsoletos.
  - **Eventos**: ratón/puntero, teclado, foco, formularios, carga, UI global, drag & drop, multimedia, portapapeles, animaciones/transiciones, sensores/dispositivo, gamepad, speech, notificaciones/push, WebRTC, Bluetooth/USB/Serial, WebXR y pagos.
- **Resumen**: “Tu diccionario maestro de superficie HTML para explotar cada rincón posible”.

### ✨ Cambiado
- N/A (versión inicial)

### 🐞 Corregido
- N/A (versión inicial)

### 📌 Notas
- Pensado para uso **offline** como catálogo maestro en bug bounty/pentesting.
