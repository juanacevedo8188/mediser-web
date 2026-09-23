# Mediser · propuesta web

Propuesta de sitio para Mediser S.R.L. (ortopedia y audiología, Sarmiento 1409, Rosario).
Un único archivo `index.html` con HTML, CSS y JavaScript sin dependencias: las tipografías
(Bricolage Grotesque y Figtree, licencia OFL) están incrustadas en el archivo.

## Vista local

```sh
python3 -m http.server 8000
```

Abrir http://localhost:8000.

## Publicar en Vercel

1. En Vercel: **Add New → Project** e importar este repositorio.
2. Framework Preset **Other**, Root Directory la raíz, Build Command vacío.
   Es un sitio estático: Vercel sirve `index.html` directamente.
3. **Deploy**. No hace falta instalar dependencias ni variables de entorno.

Cada `git push` a `main` vuelve a publicar el sitio.

## Qué incluye

- Hero animado con ondas que reaccionan al puntero y palabra rotativa.
- Tienda con filtros, vista rápida, talles y carrito que envía el pedido por WhatsApp (sin pagos online).
- Chequeo auditivo orientativo con tonos (Web Audio) que deriva a turno de audiología.
- Sección para clínicas con formulario de cotización.
- Horario en vivo, modo oscuro y selector de 3 paletas (sólo para la propuesta).

## Antes del lanzamiento

- Confirmar el WhatsApp (constante `WA` en el script); se tomó de directorios públicos.
- Reemplazar ilustraciones por fotos reales y sumar el logo original.
- Validar productos, circuito de clínicas, obras sociales y plazos marcados como "a confirmar".
- Quitar el selector de paleta y el banner de propuesta, y sacar `noindex` del `<head>`.
