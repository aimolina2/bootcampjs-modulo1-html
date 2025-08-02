# Módulo 1. HTML.

A continuación se detalla el paso a paso del ejercicio de maquetación de la página web de una tienda online.

## 1. Crear un repositorio y puesta a punto para comenzar el proyecto

Creamos el repositorio en GitHub y lo iniciamos en local.

Abrimos la carpeta en Visual Studio Code y agregamos los archivos necesarios para iniciar la práctica.

1. Creación de una carpeta **images** donde guardamos los iconos e imágenes que usaremos en el proyecto
2. Creamos el archivo **index.html** y enlazamos la hoja de estilos CSS.
3. Creamos el archivo **styles-css** que iniciamos eliminando los paddings y márgenes por defecto que aplica la hoja de estilos, así como llamando a la fuente que usaremos mediante un @import.

Con todo esto listo hacemos un primer commit y subimos los cambios a GitHub con **git add .** / **git commit -m “mensaje”** / **git push**

<img src="./images-readme/01_html_inicio.png" alt="inicio proyecto" title="inicio proyecto" />

## 2. Estructura de nuestro HTML (papel)

Con el diseño de la página a maquetar hacemos un boceto de cómo vamos a estructurar nuestro código, definiendo las etiquetas principales y contenedores.

<img src="./images-readme/02_html_boceto.png" alt="inicio proyecto" title="inicio proyecto" />

## 3. Esquema de nuestro HTML

Empezamos a montar la estructura del proyecto en el HTML creando los contenedores y etiquetas principales. Incluimos todo el contenido al que daremos estilo desde la hoja de estilos CSS.

## 4. Maquetación del contenido principal - cards de producto

En primer lugar definimos el ancho total del contenedor: 1280 px.

Antes de empezar a aplicar estilos definimos algunas de las variables que vamos a usar de forma recurrente como los colores o tamaños de fuente.

<img src="./images-readme/03_variables.png" alt="definición variables" title="definición variables" />

Maquetamos el apartado principal de **NUEVAS COLECCIONES**. Damos estilo al **h1** y trabajamos las cards que componen la grid que ocupa gran parte de la sección.

Primero usamos _flex_ para alinear en columna el título y el contenedor de todas las cards. Dentro organizamos las cards de producto con _grid_. Los valores de disposición de la grid son los que cambiamos a la hora de definir la media query (que hemos establecido como **(max-width: 920px)**), pasando de ocupar **repeat(3, 1fr)** a una única fracción **1fr**.

<img src="./images-readme/04_grid.png" alt="definición variables" title="definición variables" />
<img src="./images-readme/05_grid_responsive.png" alt="media query grid responsive" title="media query grid responsive" />

## 5. Maquetación barra de navegación

La barra de navegación ocupa toda la pantalla y se mantiene fija al hacer scroll. Usamos **flexbox** para la organización de los ítems del menú.

<img src="./images-readme/06_navbar.png" alt="barra de navegación" title="barra de navegación" />

En la declaración **@media (max-width: 920px)** donde habíamos indicado los cambios para cuando la resolución de la pantalla sea inferior a 920px añadimos las modificaciones para la barra de navegación: eliminamos los _ul_ y centramos la imagen del menú hamburguesa.
