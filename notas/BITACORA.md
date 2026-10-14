# Bitacora de JavaScript interactivo 
Laboratorio 08: JavaScript Interactivo - DOM, Eventos y Objetos. 
Navegador usado: (escribe aqui cual usaste) 
## Ejercicio 2: Seleccionar y modificar el DOM 
| Instrucción | Qué cambió en la pantalla | Se mantiene al recargar (Sí/No) |
| --- | --- | --- |
| `textContent` desde la consola | El título cambia temporalmente a "Hola desde la consola". | No |
| `textContent` desde `app.js` | El título cambia permanentemente a "Hola TECSUP". | Sí |
| `style.color` | El texto del título cambia a color azul. | Sí |
| `classList.add` | El párrafo adquiere un fondo amarillo destacado. | Sí |
| `createElement` + `appendChild` | Se añade una tercera etiqueta `<li>JavaScript</li>` a la lista. | Sí |
## Ejercicio 3: Evento click 
| Tipo de evento | Qué acción lo dispara | Cuánto suma por acción |
| --- | --- | --- |
| `click` | Un clic con el botón izquierdo del ratón. | +1 |
| `dblclick` | Un doble clic rápido en el elemento. | +1 por cada doble clic efectuado |
| `mouseover` | Pasar el puntero del mouse sobre el botón. | +1 cada vez que se ingresa con el cursor |

- **`evento.type`**: Muestra el nombre del evento que ocurrió en minúsculas (ej. `click`).
- **`evento.target`**: Retorna la referencia exacta del elemento DOM que recibió el evento (ej. `<button id="btnSumar">`).
## Ejercicio 4: Eventos input y submit 
| Prueba | Qué pasó en la pantalla | Se recargó la página (Sí/No) |
| --- | --- | --- |
| Escribir en el campo nombre | El párrafo saluda dinámicamente letra por letra. | No |
| Enviar sin `preventDefault` | Muestra brevemente el mensaje y desaparece al reiniciar la vista. | Sí |
| Enviar con `preventDefault`, correo sin `@` | Muestra el mensaje "Correo no valido: falta @" en rojo. | No |
| Enviar con `preventDefault`, correo con `@` | Muestra "Enviado: correo@ejemplo.com". | No |
## Ejercicio 5: Clases y objetos 
| Objeto | nombre | precio | `descripcion()` | `conDescuento(0.25)` |
| --- | --- | --- | --- | --- |
| `laptop` | Laptop | 2500 | Laptop - S/ 2500.00 | 1875.00 |
| `mouse` | Mouse | 45 | Mouse - S/ 45.00 | 33.75 |
| `teclado` | Teclado | 120 | Teclado - S/ 120.00 | 90.00 |
| `monitor` | Monitor | 680 | Monitor - S/ 680.00 | 510.00 |

- **Ventaja de usar Clases**: Permite encapsular atributos y métodos en una sola plantilla estructurada, evitando código duplicado[cite: 4, 11]. Permite renderizar objetos dinámicamente agregándolos simplemente al arreglo[cite: 12].
## Ejercicio 6: DOM, eventos y objetos juntos
| Prueba | Total que muestra la página | Correcto (Sí/No) |
| --- | --- | --- |
| Cuaderno 12.50 | 12.50 | Sí |
| + Lapicero 3.20 | 15.70 | Sí |
| + Mochila 89.90 | 105.60 | Sí |
| Sin `Number()` | Se interrumpe (Error en consola) | No |

| Pieza | Línea de tu código donde aparece | Para qué sirve |
| --- | --- | --- |
| **DOM** | `const listaCarrito = document.querySelector("#carrito");` | Selecciona y manipula los nodos del documento. |
| **Evento** | `formProducto.addEventListener("submit", ...)` | Escucha la interacción cuando el usuario envía el formulario. |
| **Objeto** | `const producto = new Producto(...)` | Crea e instancia un objeto de datos reutilizable. |