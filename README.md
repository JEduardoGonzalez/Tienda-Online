# Tienda-Online

### Funciones definidas en el código Tienda.js

**Función agregarProductoAlCarrito.**
Se ejecuta cuando se presiona el botón agregar de cualquier producto, lo que hace es buscar que el producto a agregar no esté dentro de un arreglo llamado carrrito, si el producto no está lo agregará a carrito, pero si el producto ya está guardado en carrito, aumentará la cantidad del producto, sumando la cantidad guardada con la que se desea agregar.
**Función actualizarResumenCompra.**
Se ejecuta despues de la función agregarProductoAlCarrito, primero que nada limpia el interior de una tabla llamado resumencompra para evitar repetir datos al ejecutarse varias veces. Por cada producto dentro del carrito creará un registro que incluye id, descripción, cantidad, precio y subtotal, estos registros se guardarán en una variable fila y esta a su vez se guardará en resumencompra. Cada subtotal será sumado para conformar el total de la compra, cuyo valor se verá representado en el elemento total, el cual siempre se verá al final de la tabla.

### ¿qué tipo de variable es "catalogo" en el código js y cómo se manipula ?
Se tratá de un arreglo que contiene una coleccion de datos, simulando productos con los atributos id, imagen, precio y descripcion. Dicho arreglo se utiliza en un ciclo que crea un contenedor para cada producto, por lo que si existen 10 productos se crearán 10 contenedores, si existen 0 productos entonces no se crearán contenedores.

### ¿Que hace const card = document.createElement("div") ?
Crea un nuevo elemento HTML de tipo "div" y lo almacena en una variable llamada "card".

### ¿Que hace card.innerHTML ?
Se utiliza para acceder y modificar el contenido HTML interno de un elemento, en este caso, el que está almacenado en la variable card.
### ¿Que hace catalogoContainer.appendChild(card) ?
Se utiliza para agregar un elemento (en este caso, el elemento "card") como hijo de otro elemento (el elemento "catalogoContainer").
