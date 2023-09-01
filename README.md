# Tarjeta giratoria de producto 

En este ejercicio se realiza una tarjeta de producto que gira y muetsra informacion adicional de un producto.

En este ejercicio se hace uso de las transformaciones 3d con CSS

- Se utiliza el objeto *div.flip-card* como contenedor de toda nuestra tarjeta.

- El objeto *div.flip-card-inner* toma el rol de la tarjeta fisica a la que se le aplicara la transformacion de rotacionY(180deg)
	- Con la propiedad transition se establece el tiempo que le tomara realizar la transformacion
	- Con la propiedad *transform-style: preserve-3d* establecemos que los elemntos hijos sigan en el espacio 3d

- Se establece que al recibir la acion 'hover' el elemento *div.flip-card-inner* realizara la rotacionY(180 grados).

- Se crean 2 elementos div, uno para la cara frontal (*flip-card-front*) y otra para el reverso de la tarjeta (*flip-card-back*). ambas con dimenciones de 100%,100% posicion absoluta y *backface-visibility: hidden*, para que no se muestre cuando estan de espaldas.

- Se inicia aplicando a la cara trasera una rotacionY(180 grados), de modo que comienza de espaldas y no es visible.

-Cuando se desencadena la transformación el elemento *.flip-card-inner* (que contiene ambas caras) realiza su rotacion, la cara front ahora queda de espaldas por lo que se oculta, la cra back queda de frente, por lo que ya es visible.