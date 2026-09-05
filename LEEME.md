# TOTAL HANDS · Estación de Gestos

App de una sola página que usa la cámara y detecta tus manos (21 puntos por mano)
para presentar el combo **TRIO MALETERO DRYWALERO 5.0** sin tocar nada.
Todo se procesa en el navegador: el video **no sale** de la computadora.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La app completa (HTML + CSS + JS en un solo archivo) |
| `combo-1.jpg` | Imagen 1 del combo (ya optimizada) |
| `combo-2.jpg` | Imagen 2 del combo (ya optimizada) |

## Subirlo a GitHub Pages desde el celular

1. GitHub → tu repo → **Add file → Upload files**.
2. Sube los **tres** archivos juntos (index.html, combo-1.jpg, combo-2.jpg) y haz commit.
3. **Settings → Pages** → Branch `main` / carpeta `/ (root)` → Save.
4. Abre `https://TU-USUARIO.github.io/TU-REPO/` y dale **Permitir** a la cámara.

> La cámara **solo funciona en `https://`** (o en `localhost`). GitHub Pages ya es https, así que va bien.
> Si lo abres como archivo local (`file://`) el navegador no te dará la cámara.

## Gestos

| Gesto | Qué hace |
|---|---|
| ✋ Palma abierta | Muestra u oculta la ficha del combo |
| 👉 Deslizar la mano abierta | Cambia de imagen |
| 🤏 Pinza (pulgar + índice) | Agarra y mueve el producto |
| 🤏🤏 Dos pinzas | Agranda, achica y rota |
| ✊ Puño | Carga energía; abre la mano y explota |
| ☝️ Índice | Dibuja con luz en el aire |
| ✌️ Paz | Cambia de modo |
| 👍 Pulgar arriba | Saca el número de WhatsApp |

**Modos:** Combo · Efectos · Modo AR (el combo se pega a tu mano) · Rayos X.

**Teclas:** `G` guía · `S` foto · `F` pantalla completa · `M` sonido · `Espacio` modo · `←/→` imagen · `C` ficha · `W` WhatsApp.

## Cambiar el combo

- **Rápido:** botón 🖼️ (o arrastra imágenes a la ventana). Carga hasta 8 imágenes desde la PC, sin tocar código.
- **Permanente:** reemplaza `combo-1.jpg` / `combo-2.jpg`, o edita el array `SLIDES` arriba del script
  (`title`, `sub`, `specs`) y la constante `PRICE`.

## Datos técnicos

- Detección de manos: **MediaPipe Tasks Vision 0.10.14** (se descarga de jsDelivr la primera vez y queda en caché).
- Necesita internet la primera vez para bajar el modelo (~7 MB); después funciona con el caché del navegador.
- Si algo falla con la cámara, el botón **Ver sin cámara** entra igual en modo demo (se controla con el mouse).
- Probado con Chromium: los 6 gestos clasifican correctamente y la captura de foto (📸) descarga un PNG.

---
Total Tools · Herracast S.A.C. · totaltoolspe.com · WhatsApp 933 724 178
