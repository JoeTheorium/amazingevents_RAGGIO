# amazingevents_RAGGIO
// Este código JavaScript nos permite filtrar eventos por categoría o por palabra clave.
// Además, podemos ver los eventos disponibles y hacer "click" en el botón para ir a los detalles de cada uno.

// En primer lugar, se importa un archivo con la información de los eventos que se van a mostrar.
// Después, se crea un fragmento de documento, que se utiliza para agregar elementos al DOM (el árbol de objetos que representa la estructura de una página web).
// Se definen dos funciones principales, una para crear las tarjetas de eventos y otra para filtrarlos.
// La función "createCards" toma como argumento un array de eventos y un contenedor donde se van a mostrar.
// Esta función vacía el contenido del contenedor y, a continuación, recorre el array de eventos para agregar una tarjeta por cada uno.
// Cada tarjeta se crea como un elemento article con una imagen, un título, una descripción, un precio y un botón que lleva a los detalles del evento.
// Por último, si NO hay eventos disponibles, se muestra un mensaje que indica que NO se encontraron eventos.
// La función "filterByCategory" toma como argumento un array de eventos y un texto que indica la categoría que se quiere filtrar.
// Esta función filtra el array de eventos para devolver solo aquellos que pertenecen a la categoría que se especificó.
// En el siguiente bloque de código, se obtienen las categorías únicas de los eventos y se crean elementos de formulario (etiquetas y casillas de verificación) para cada una de ellas.
// Luego, se agregan estos elementos al DOM. Después, se define una variable filters que es una copia del array de eventos.
// Esto es necesario para que la función de búsqueda NO afecte al array original.
// La función "filterByKeyword" filtra los eventos por palabra clave, tomando como argumento el array de eventos y la palabra clave.
// Devuelve un array con los eventos que coinciden con la palabra clave.
// A continuación, se define una variable "$search" que hace referencia al campo de entrada de búsqueda en el formulario.
// Se agregan dos escuchadores de eventos a este campo, uno para escuchar cambios en el valor del campo y otro para escuchar envíos del formulario.
// Cada vez que se escribe algo en el campo de búsqueda, se llama a la función "filterByKeyword" con los filtros actuales y la palabra clave escrita.
// La nueva lista de eventos filtrados se pasa a la función "createCards" para que se muestren en la página.
// Finalmente, cuando se envía el formulario, se llama a la función "filterByKeyword" con los filtros actuales y la palabra clave escrita, y se muestra la lista de eventos filtrados.
// Por último, se exporta la función "createCards".
