# Guía Básica de CSS Font

## ¿Qué es la propiedad `font` en CSS?

La propiedad `font` en CSS nos permite controlar cómo se ve el texto en una página web. Con ella podemos cambiar el tipo de letra (tipografía), el tamaño, el peso (grosor), el estilo (normal o cursiva) y más.

---

## Propiedades más usadas para fuentes en CSS

- **font-family**: Define la tipografía que usará el texto.
  ```css
  font-family: Arial, Helvetica, sans-serif;
  ```
  Puedes poner varias fuentes separadas por comas. Si el navegador no encuentra la primera, usará la siguiente.

- **font-size**: Cambia el tamaño del texto.
  ```css
  font-size: 16px;
  ```

- **font-weight**: Cambia el grosor del texto.
  ```css
  font-weight: bold; /* o valores numéricos como 400, 700, etc. */
  ```

- **font-style**: Cambia el estilo del texto (normal, italic, oblique).
  ```css
  font-style: italic;
  ```

- **line-height**: Cambia el espacio entre líneas de texto.
  ```css
  line-height: 1.5;
  ```

---

## Ejemplo básico

```css
body {
  font-family: 'Arial', sans-serif;
  font-size: 18px;
  font-weight: 400;
  font-style: normal;
  line-height: 1.6;
}
```

---

## Usando fuentes externas

Puedes usar fuentes que no están instaladas en tu computadora, como Google Fonts o archivos `.ttf` que tengas en tu proyecto.

### Google Fonts

1. Ve a [Google Fonts](https://fonts.google.com/).
2. Elige una fuente y copia el enlace `<link>` en el `<head>` de tu HTML.
3. Usa la fuente en tu CSS con `font-family`.

```html
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
```
```css
body {
  font-family: 'Roboto', sans-serif;
}
```

### Fuentes locales con `@font-face`

Si tienes un archivo de fuente (por ejemplo, `Exile-Regular.ttf`), puedes usarlo así:

```css
@font-face {
  font-family: 'MiFuente';
  src: url('./Fuentes/Exile-Regular.ttf');
  font-weight: normal;
  font-style: normal;
}

h1 {
  font-family: 'MiFuente', sans-serif;
}
```

---

## Buenas prácticas

- Siempre pon una fuente de respaldo (por ejemplo, `sans-serif`).
- Usa tamaños de fuente legibles (mínimo 16px para el cuerpo del texto).
- No uses demasiadas fuentes diferentes en una misma página.

---

## Recursos útiles

- [Documentación de MDN sobre font](https://developer.mozilla.org/es/docs/Web/CSS/font)
- [Google Fonts](https://fonts.google.com/)

---

¡Sigue practicando y experimentando con diferentes fuentes para mejorar el diseño de tus páginas web!