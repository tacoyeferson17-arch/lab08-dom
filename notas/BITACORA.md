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
## Ejercicio 6: DOM, eventos y objetos juntos
