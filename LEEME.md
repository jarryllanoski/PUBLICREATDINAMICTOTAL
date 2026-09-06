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
| 🙌 **Las dos manos** | **Abre las 2 imágenes a la vez**, una a cada lado |
| ✋ Palma abierta | Muestra u oculta la ficha del combo |
| 👉 Deslizar la mano abierta | Cambia de imagen |
| 🤏 Pinza (pulgar + índice) | Agarra y mueve el producto **o saca una pieza** |
| 🤏🤏 Dos pinzas | Agranda y rota (o sacas **dos piezas a la vez**, una por mano) |
| ✊ Puño | Carga energía; abre la mano y explota (en modo Piezas desarma todo) |
| ☝️ Índice | Dibuja con luz en el aire |
| ✌️ Paz | Cambia de modo |
| 👍 Pulgar arriba | Saca el número de WhatsApp |

**Modos:** Combo · **Piezas** · **Iron Man** · Efectos · Modo AR (el combo se pega a tu mano) · Rayos X.

**Teclas:** `G` guía · `S` foto · `V` grabar · `J` voz · `F` pantalla completa · `E` encuadre · `R` rearmar · `M` sonido · `Espacio` modo · `←/→` imagen · `C` ficha · `W` WhatsApp.

## Modo IRON MAN 🦾

Interfaz tipo JARVIS **con voz en español**: corchetes de pantalla, línea de barrido,
retículas giratorias sobre cada mano, telemetría en vivo y consola que escribe lo que va diciendo.

- A cada lado aparece un **riel con toda tu lista de imágenes**.
- **Pinza sobre un ítem del riel izquierdo → lo saca tu mano izquierda; el riel derecho, tu mano derecha.**
  Cada mano sostiene su propio holograma y lo mueve por la pantalla; los dos a la vez.
- **✊ Puño** con esa mano → devuelve su holograma al riel.
- **✋ Palma** → abre la ficha y **la voz lee el combo y el precio**.
- **👍 Pulgar** → la voz dicta el número de WhatsApp.
- Botón **🗣️** (tecla `J`) enciende y apaga la voz. Usa la voz en español que tenga tu
  navegador; en Chrome de escritorio y Android ya viene instalada.

### Tu lista de imágenes

La app busca `combo-1.jpg`, `combo-2.jpg`, `combo-3.jpg` … hasta `combo-8.jpg` y usa las que existan.
**Para sumar imágenes solo súbelas al repo con ese nombre** — aparecen solas en los rieles, en el
carrusel y en el despiece. También puedes cargarlas al vuelo con 🖼️ o arrastrándolas.

## Grabar pantalla 🎥

Botón **⏺** (tecla `V`) empieza y para la grabación. Graba el lienzo en **1080p / VP9**
y, si le das permiso, **suma el micrófono** para que se escuche tu voz y la de JARVIS.
Sale un indicador **REC** con el cronómetro, y al parar se descarga un `.webm`.
Si tu navegador bloquea la descarga automática, aparece el botón **💾 Guardar video** —
un clic y se guarda. Los botones y la guía **no salen en el video**, solo la imagen limpia.

> Probado: video de 1280×720 VP9 + audio Opus, archivo válido y reproducible.

## Modo PIEZAS (sacar pieza por pieza)

Al entrar al modo, la app **despieza sola** la imagen: rellena el fondo desde los bordes
y separa cada objeto que queda (herramienta, batería, maletín, el "2049", los regalos…).
En las dos imágenes del combo salen **18 y 17 piezas**.

- Haces **pinza sobre una pieza** y la sacas del cartel; queda un hueco oscuro en su lugar.
- Con **las dos manos sacas dos piezas al mismo tiempo**, cada una por su lado.
- La pieza agarrada se agranda y brilla; al soltarla se queda flotando donde la dejaste.
- ✊ **Puño** = desarma todo de golpe. **🧩 / tecla `R`** = vuelve a armar el combo.
- Funciona con **cualquier imagen** que cargues (botón 🖼️). Si una imagen no se puede
  despiezar (fondo muy mezclado), la corta en cuadrícula de 16 para que igual puedas moverla.

## Dos manos = las dos imágenes

En modo **Combo** y **Efectos**, en cuanto la cámara ve **las dos manos**, la imagen se abre
en dos: la 1 a la izquierda y la 2 a la derecha, cada una con su rótulo. La ficha del precio
se aparta sola para no tapar. **Cada mano arrastra su propia imagen** haciendo pinza.
Al bajar una mano vuelve solo a una imagen.

## Guía de gestos

Botón **✋** (o tecla `G`) la muestra y la oculta; también se cierra tocándola.
El botón queda encendido cuando la guía está visible. Al abrir la app se muestra sola
20 segundos y luego se esconde; si tú la abres, se queda hasta que la cierres.

## Encuadre

Botón **📐** (o tecla `E`): alterna entre
- **Completo** (por defecto): se ve todo el cuadro de la cámara, sales entero, con las capas encima.
- **Pantalla llena**: el video llena la pantalla recortando los bordes.

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
