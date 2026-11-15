# Portfolio

Web personal: sobre mí, proyectos y notas.

- `index.html` contiene toda la web: una sola página con secciones y rutas por `#`.
- `imagenes/` guarda las fotos. Si una foto no existe todavía, el hueco se queda limpio y la web sigue funcionando.

## Añadir contenido

Todo se edita en los dos arrays de JavaScript al final de `index.html`:

- `PROYECTOS`: cada entrada tiene `titulo`, `year`, `url`, `foto`, `desc` y `tags`.
- `NOTAS`: cada entrada tiene `slug`, `titulo`, `subtitulo`, `fecha`, `tipo`, `lectura`, `portada` y `cuerpo`.

Los bloques disponibles para el cuerpo de una nota:

```js
{p:"párrafo"}
{h:"subtítulo"}
{cita:"frase destacada"}
{foto:"imagenes/x.jpg", pie:"texto", ancha:true}
{duo:["imagenes/a.jpg","imagenes/b.jpg"], pie:"texto"}
```

## Tamaños de imagen recomendados

| Uso | Proporción | Ancho sugerido |
|---|---|---|
| Retrato de inicio | 4:5 | 900 px |
| Miniatura de proyecto | 4:3 | 800 px |
| Portada de nota | 1:1 | 700 px |
| Foto dentro de un artículo | 3:2 | 1400 px |
| Foto ancha de artículo | 16:9 | 2000 px |

## Publicar en GitHub Pages

1. Subir el repo a GitHub.
2. Settings → Pages → Source: `Deploy from a branch`, rama `main`, carpeta `/ (root)`.
3. La web queda en `https://<usuario>.github.io/<repo>/`.
