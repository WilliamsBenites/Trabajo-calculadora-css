# Calculadora
- Color de fondo: background-color: rgb(7, 94, 7); - Establece el color de fondo del elemento a un verde oscuro.

Borde: border: 3px solid rgb(0, 0, 0); - Crea un borde negro sólido de 3 píxeles alrededor del elemento.

Esquinas redondeadas: border-radius: 20px; - Hace que las esquinas del borde sean redondeadas.

Dimensiones: width: 400px; y height: 400px; - Establece que el ancho y la altura del elemento sean de 400 píxeles.

## PADDING:
- padding-top: 20px;
padding-left: 40px;
padding-right: 20px;
padding-bottom: 40px;

Estos valores añaden espacio interno (relleno) alrededor del contenido del elemento: 20 píxeles arriba, 40 a la izquierda, 20 a la derecha y 40 abajo.

### FLEXBOX
- display: flex; - Activa el modelo de diseño flexible, lo que permite       alinear los elementos internos de manera más fácil.

- align-items: center; - Alinea verticalmente los elementos internos al centro del contenedor.

- justify-content: center; junto con el código que mencionaste anteriormente, todos los elementos dentro del cuadro verde se centrarán horizontalmente, 
- además de que ya estaban alineados verticalmente con  align-items: center;. Esto crea un efecto de centrado tanto vertical como horizontal.

|| flex-wrap: wrap; ::
    Esta propiedad se utiliza en un contenedor flexible (con display: flex;) y determina cómo se comportan los elementos hijos cuando no hay suficiente espacio en una sola línea.
    
 -  Al establecerlo en \\wrap\\, le indicas al contenedor que si los elementos  no caben en una sola línea, deben "envolverse" a la siguiente línea. 

 ### GRID
 - display: grid; ::
    Activa el modelo de diseño de cuadrícula (grid) para el elemento. Esto significa que el contenedor se dividirá en filas y columnas, permitiendo una disposición más estructurada de los elementos hijos.
 - grid-template-columns: repeat(3, 1fr);::
    Define el número y el tamaño de las columnas en la cuadrícula
    1fr: Significa "una fracción". Así que cada columna ocupará una fracción igual del espacio disponible en el contenedor.