# Lumen · Reproductor de mi biblioteca

Reproductor de música de un solo archivo (`index.html`), sin servidor ni dependencias. Funciona con los archivos de audio de tu propio equipo, con una interfaz de vidrio esmerilado cuyos colores se adaptan a la carátula de cada canción.

> **Privacidad:** el reproductor no hace ninguna petición de red. Tu música nunca sale de tu equipo y no se sube a ningún lugar.

## Características

- **Biblioteca local:** elige archivos sueltos o una carpeta completa, o arrástralos a la ventana. Formatos: MP3, M4A, FLAC, OGG, WAV, AAC y Opus (según lo que admita tu navegador).
- **Etiquetas y carátulas:** lee título, artista, álbum y carátula de los MP3 con etiquetas ID3v2.3/2.4. Los colores de acento salen de la carátula. Sin etiquetas, usa el nombre del archivo (`Artista - Título.mp3`).
- **Biblioteca persistente:** en Chrome y Edge recuerda la carpeta elegida. Guarda también la última pista, el segundo donde quedaste, el volumen y el modo aleatorio.
- **Ecualizador real:** las barras y el brillo del fondo reaccionan a la música.
- **Control de reproducción:** aleatorio, repetir (lista o pista), cola editable, velocidad (0,75× a 2×) y temporizador de apagado.
- **Lista:** búsqueda, filtro de “me gusta” y agrupación por álbum.
- **Integración con el sistema:** teclas multimedia y controles de la pantalla de bloqueo.
- **Accesibilidad:** respeta la preferencia de reducir movimiento.

## Cola de reproducción

Pasa el cursor sobre una canción y pulsa **＋** para añadirla a continuación. En las canciones en cola aparece **▸ n ✕**: púlsalo para quitarla. El botón **▸ n ✕** de la fila de herramientas vacía toda la cola. También sirve el clic derecho.

## Atajos de teclado

| Tecla | Acción |
|---|---|
| Espacio | Reproducir / pausar |
| N / P | Siguiente / anterior |
| ← / → (en la barra de progreso) | Retroceder / avanzar 5 s |
| ↑ / ↓ | Volumen |
| L | Me gusta |
| S | Aleatorio |
| R | Repetir |
| M | Silenciar |
| / | Ir a la búsqueda |

## Navegadores

| Función | Chrome / Edge | Firefox / Safari |
|---|---|---|
| Reproducción, cola, búsqueda, atajos | Sí | Sí |
| Recordar la carpeta entre sesiones | Sí | No (hay que elegirla cada vez) |
| Ecualizador en tiempo real | Sí | Parcial (Safari usa barras animadas) |

## Publicar con GitHub Pages

1. Crea un repositorio y sube estos archivos a la rama `main`.
2. En el repositorio: **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/ (root)` y guarda.
4. En unos minutos estará disponible en `https://<tu-usuario>.github.io/<nombre-del-repositorio>/`.

## Estructura

```
index.html   El reproductor completo (HTML, CSS y JavaScript)
.nojekyll    Indica a GitHub Pages que sirva el archivo tal cual
.gitignore   Evita subir archivos de audio por accidente
README.md    Este documento
```

## Limitaciones conocidas

- No lee etiquetas de M4A, FLAC ni OGG (usa el nombre del archivo).
- No hay reproducción sin pausas ni crossfade entre pistas.
- La velocidad, la repetición y la cola no se conservan al cerrar la pestaña.
- Los datos guardados (carpeta, “me gusta”, última pista) viven en el navegador y se asocian al dominio donde se publique.

## Licencia

Pendiente de definir por el autor.
