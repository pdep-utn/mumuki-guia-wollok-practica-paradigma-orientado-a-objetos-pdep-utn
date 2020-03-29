Queremos hacer un sistema para hacer compras online de modo que se puedan agregar productos al carrito de compras, y saber cuánto se debería abonar por la compra cuando sea necesario.

Requerimientos y cosas a tener en cuenta:

- Necesitamos poder **agregar productos al carrito**, considerando que debe ser posible agregar un mismo producto al carrito varias veces, lo cual implica que se desea comprar esa cantidad del producto en cuestión.
- Queremos poder determinar:
  - si el carrito **está vacío**, que se cumple cuando no se le agregó ningún producto;
  - **cuántos productos hay** en el carrito en total (considerando aquellos que fueron agregados más de una vez).
- Necesitamos saber cuál es el **total a abonar** por los productos agregados al carrito.

A los distintos productos nos interesa poder configurarles su **descripción** y el **precio unitario**, de modo que esa información pueda usarse para los requerimientos explicados. Por ejemplo, un producto podría tener como descripción `"Aceite de girasol"` y como precio unitario el valor `60.75`.

Ejemplos de uso:

```Wollok
ム carrito.agregar(producto)
ム carrito.estaVacio()
ム carrito.cantidadDeProductos()
ム carrito.totalAAbonar()
```