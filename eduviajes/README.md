# Edu Viajes · propuesta web

Propuesta de sitio para Edu Viajes (viajes y turismo, 9 de Julio 1117, Rosario · sucursal Maciel · EVT Leg. 12931).
Un único archivo `index.html` con HTML, CSS y JavaScript sin dependencias: las tipografías
(Fraunces, Schibsted Grotesk y Caveat, licencia OFL) están incrustadas en el archivo.

## Vista local

```sh
cd eduviajes && python3 -m http.server 8000
```

## Publicar en Vercel

Crear un proyecto nuevo importando este repositorio con **Root Directory = `eduviajes`**,
Framework Preset **Other** y Build Command vacío. Así queda separado del sitio de Mediser.

## Qué incluye

- Identidad estrictamente verde y blanca (ilustraciones incluidas, generadas del tono elegido), con notas manuscritas y cursivas subrayadas a mano que se dibujan al aparecer.
- Hero animado: avión que sale del Monumento a la Bandera, parallax, cartel split-flap y sello giratorio.
  En modo oscuro el cielo pasa a noche con estrellas.
- Tablero de salidas tipo aeropuerto (fechas de ejemplo) que abre la ficha del viaje.
- Catálogo de 13 destinos en formato polaroid con ilustraciones animadas, filtros por región y perfil, y mapa con rutas desde Rosario.
- Sección colegios: niveles en pestañas de carpeta, qué incluye en una hoja de cuaderno, recorrido paso a paso con un micro que avanza al scrollear y formulario a WhatsApp.
- Simulador de cuotas (fija o indexada) con valor en pesos de hoy, gráfico y tabla.
- Cotizador que arma una tarjeta de embarque en vivo y envía la consulta por WhatsApp o email (sin pagos online).
- Reseñas como postales con estampilla y matasellos.
- Horario en vivo, modo oscuro y selector de 3 tonos de verde para elegir el de la marca (sólo para la propuesta).
- Respeta `prefers-reduced-motion`.

## Antes del lanzamiento

- Confirmar el WhatsApp (constante `WA`) y los horarios (`HRS`); se tomaron de directorios públicos o son supuestos.
- Dirección de Maciel, razón social y habilitación de turismo estudiantil (Ley 25.599).
- Reemplazar destinos, itinerarios, salidas (`DESTS`, `DEPS`) y reseñas de ejemplo por los reales.
- Ajustar el verde al código exacto de la marca, sumar logo y fotos reales; quitar el banner y el selector de paleta y sacar `noindex` del `<head>`.
