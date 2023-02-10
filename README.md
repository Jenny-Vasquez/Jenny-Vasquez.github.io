# Jenny-Vasquez.github.io
PAra el proyecto he utilizado las siguientes herramientas.

Animación menú:

   .enlaces a:hover {
    border-bottom: 1px solid;
    background: #eabbd4;
    border-radius: 10px;
Para que subrayar el enlace si el cursor pasa por encima del mismo.

Animacion de imagenes:

Para las tarjetas: he creado la clase galeria que contiene la capa contenedora donde estara la imagen,
a estas le he aplicado los siguientes atributos.


 .Galeria .contenedor {
    position: absolute;
    width: 30%; 
    margin-top: 30px;
    margin-left: 50px;
    float:left; 
}
.Galeria .contenedor img {
    position: absolute;
    left: 30px;
    transition: opacity 1.5s ease-in-out; ----------> el tiempo de transicion entre ambas imagenes
    border-radius: 80px;
    width: 350px;
    height: 450px;
  }
  .Galeria .contenedor img.top:hover {
    opacity: 0;
Carrusel:
Lo he utilizado para presentar varias imagenes y que estas se muevan segun el usuario mueva el cursor.
para ello he utilizado varias capas para que contenga la galeria de imagenes. A estas le he aplicado los siguientes atributos.

 .Galeria .Fotos {
    display: flex; ------> distribuye de forma prporcional las images dentro de la capa contenedora
    position: absolute;
    width: 650px;
    height: 550px;
    margin-top: 50px;
    margin-left: 15px;
    float:left; 
}
.Galeria .Fotos img {
    width: 0px;
    flex-grow: 1;
    object-fit: cover; -----------> redimensiona la imagen para ajustarse a su contenedor.
    opacity: .8;
    transition: 2s ease; -----> tiempo de transición entre fotografias
    border-radius: 10px;
  }
  .Galeria .Fotos img:hover {
    cursor: crosshair;------->cambio de cursor
    width: 300px;
    opacity: 1;
    filter: contrast(120%);
  }
