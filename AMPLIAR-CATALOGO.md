# Agregar más productos

El diseño actual usa `dist/blue-studio.css` y `dist/blue-studio.js`. La cuadrícula añade filas automáticamente según el número de productos; no hay un límite fijo de siete tarjetas.

Para ampliar el catálogo, guardar la fotografía individual dentro de `dist/assets` y agregar un objeto en `additionalProducts` de `dist/config.js`:

```js
{
  id: 'identificador-unico',
  name: 'Nombre real del producto',
  category: 'Planchas', // Planchas, Secadoras, Rizadores o Barbería
  image: 'nombre-de-la-imagen.png',
  desc: 'Descripción breve del producto',
  features: ['Característica verificada', 'Otra característica']
}
```

Agregar su precio en MXN dentro de `prices`, usando el mismo identificador como clave. Los nuevos productos aparecerán en el catálogo, buscador, categoría, detalle y carrito. Usar identificadores simples sin espacios o símbolos especiales y nombres de archivo correspondientes a imágenes locales. Para nuevas categorías, actualizar el arreglo `groups` y los filtros de la página.

Los espacios editoriales y de distribución acompañan a los productos reales; no representan inventario o productos inexistentes. El pago real y el contacto siguen pendientes según lo solicitado por el propietario.

