# bootstrap-website

<!--My fonts-->
pagina google: https://fonts.google.com

# Escogiendo mi navegacion 
<!--NAVIGATION-->
1. Para mi navbar use NAV porque es responsive.

2. Para mover al lado derecho le agregamos una clase llamada margin (margen) en el nav ml-auto en las <ul> que contiene las <li>
ejemplo:  <ul class="navbar-nav ml-auto">

3. Eliminamos el <span> de home.
4. agregamos un about en lugar del feature.
5. Agregamos espaciado en los lados para centrar el contenido. y agregamos un contenedor con un <div> de clase container. y asi centramos.


# Realizando la seccion HEADER. Una nueva navegacion.
<!--HEADER-->
Esto es para que el usuario navegue en distintas secciones.
1. Agregamos un contenedor de bootstrap en 2 partes (dos columnas de bootstrap) para dividir el contenido a la mitad.
2. La imagen debe tener el mismo nombre como la guardaste. Para que se vea completa le colocamos un style de 100% y una clase de margen top de el tamaño que prefieras. En mi ejemplo utilice un 
<div class="container mt-5">

3. El texto
Dentro de las columnas coloque unos div de clase header para el contenido de la izquierda. colocamos nuestro titulo con <h1> y un parrafo <p> y un botton.
<a hrf="# class="btn btn-outline-secundary btn-lg"> btong lg es para hacerlo mas largo. tambien podemos añadir un margin top.
Para colocar el titulo cercano a la imagen le agregamos u <h1 class="display-4"

# Seccion de testimonios
<!--TESTIMONIOS-->
Le agregamos un usuario y un Id
 <p class="mb-2"> sigue viendose encima
Lo estilizamos cambiando el tamaño del autor. con un <h3>
y el parrafo <h2>
Alteramos con el css para mejorarlo.

# Seccion de informacion.
<!--INFO ONE-->
Separar contenido de derecha a izquierda creando filas y columnas. (2 columnas de 6 que conforman las 12 de bootstrap).
Nota: Las filas solo funcionan dentro de una fila de bootstrap por ellos agregamos las columnas. Para centrar la imagen en la seccion coloco un margen en el eje "y" columnas. en mi div container agrego <div class="col-md-6 my-auto">

<!--INFO TWO-->
Quiero bajar y que la barra de navegacion (navigation) siempre se vea. Para ello le agrego a la clase de bootstrap un fixed-top.
ejemplo:
<nav class="navbar navbar-expand-lg navbar-light bg-light fixed-top">

Asi mismo, el header que no se vea encimado. Para ello en nuestro archivo de css le cambiamos los px para el espaciado inclusive si usas medias querys podrias hacerle un mejor trabajo. ver archivo del sgte ejemplo: 

header {
      75 px
}

Agregando un color a nuestra sección:
<section id="info-two" style="background: #f1f1f1;">

<!--FOOTER-->
Footer o seccion final. Linkear con la navegación.
Hacemos solo una columna de 5 (para luego hacer un espaciado) y una tarjeta que es algo que bootstrap crea (un cuadrado blanco), este contenido sera un formulario, es la clase tarjeta.    
<form class="card"> --> Aqui adentro tendra una trajeta body.

<div class="card-body"> --> dentro del body estaaran los inputs tipo text.
pare ello hago un input con placeholder de tipo texto con lo que debe cargarse adentro.
 <div class="form-group">
      <input type="text" class="form-control" placeholder="Name">
</div>

//Repetimos lo anterior para email

Para la seccion de mensaje hacemos un <textarea> 

para un boton del tamaño de mi cuadro le agrego el btn-block

<button class="btn btn-outline-secondary btn-block">

# Footer: 
Añadimos un background en nuestro archivo css con la imagen que queremos mostrar.

# Animaciones:
Esta la realizamosd en la seccion de script. (tambien podrias hacerlo en un archivo de .js por separado).

Adicionalmente el scroll lo guardamos en una variable de windows y lo realizamos para cada seccion que se desee animar: 

window.sr = ScrollReveal(); 
Esto es solo un metodo que luego vamos a configurarlo. Lo que hace el metodo es seleccionar un elemento y realizar una navegacion (ver seccion de <script>)

veamos el sgte ejemplo con navbar:

sr.reveal('.navbar', {
  duration: 2000,
  origin: 'bottom'
});

Por ultimo: Para no cambiar el contenido de forma brusca utilizaremos Scrolling-StackOverflow:
Documentación: https://stackoverflow.com/questions/7

Con esta Jquery observamos como se desliza entre distintas secciones.

-Fin-

