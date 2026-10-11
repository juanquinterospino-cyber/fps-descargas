# Avisos de software de terceros

FPS incluye los siguientes componentes de terceros. Cada uno conserva su propia licencia.

## FFmpeg

FPS ejecuta FFmpeg como un **programa independiente** (un archivo ejecutable dentro de `resources/bin/`, al lado de la aplicación). FPS no está enlazado a las bibliotecas de FFmpeg.

Los instaladores incluyen estas compilaciones, ambas de FFmpeg **6.1.1** y con licencia **GNU GPL**:

| Instalador | Compilación | Origen |
|---|---|---|
| macOS (Intel y Apple Silicon) | `6.1.1-tessus` | https://evermeet.cx/ffmpeg/ |
| Windows | `6.1.1-essentials_build-www.gyan.dev` | https://www.gyan.dev/ffmpeg/builds/ |

Los binarios se obtuvieron a través del paquete [ffmpeg-static](https://github.com/eugeneware/ffmpeg-static) (versión de binarios `b6.1.1`).

**Código fuente.** FFmpeg es software libre. Su código fuente correspondiente a la versión 6.1.1 está disponible en:

- https://ffmpeg.org/download.html (sección *Releases*, versión 6.1.1)
- https://github.com/FFmpeg/FFmpeg (etiqueta `n6.1.1`)

Las compilaciones usan además bibliotecas propias con licencia GPL, entre ellas **x264** (https://www.videolan.org/developers/x264.html), cuyo código fuente está en https://code.videolan.org/videolan/x264. La configuración exacta de cada compilación se ve con el comando `ffmpeg -version` sobre el ejecutable incluido.

Si necesitas el código fuente y no logras encontrarlo en esos enlaces, escríbenos a través de [ascensodigital.cl](https://ascensodigital.cl).

Textos de licencia en esta carpeta: [`licencias/ffmpeg-LICENSE.md`](licencias/ffmpeg-LICENSE.md) y [`licencias/ffmpeg-windows-build-info.txt`](licencias/ffmpeg-windows-build-info.txt) (descripción de la compilación de Windows). El texto completo de la GPL está en https://www.gnu.org/licenses/gpl-3.0.html.

## Electron

FPS está construido sobre [Electron](https://www.electronjs.org/) (licencia MIT), que incluye Chromium y Node.js. Los avisos de licencia de sus componentes van dentro de cada instalador (archivos `LICENSE` y `LICENSES.chromium.html` junto a la aplicación).

## Otras bibliotecas

- [fluent-ffmpeg](https://github.com/fluent-ffmpeg/node-fluent-ffmpeg) — MIT
