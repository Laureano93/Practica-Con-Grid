# Practica Con Grid

- Descripcion Del Proyecto
- Desarrollo Del Proyecto
- Visualizacion Del Proyecto
- Enlaces
- Licencias

---

**Descripcion Del Proyecto**

*Consisten en realizar una pagina web donde se muestra un header(con su
correspondiente informacion), un nav donde se muestra un menu junto con 2 imagenes
con un comentario debajo.
Debajo 3 fotos alineadas con respecto a las 2 de arriba y un footer debajo donde muestro
las redes sociales, licencia y ubicacion de las fotos. Todo esto empleando contenedores y
css3 para que mediante el uso de Grid  se queden alineadas y tenga una buena maquetacion*

## Desarrollo Del Proyecto
*Mediante el visual studio code desarrollo un archivo html que contiene:*

~~~
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Laureano Guillen Dil">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.15.1/css/all.css" integrity="sha384-vp86vTRFVJgpjF9jiIGPEEqYqlDwgyBgEF109VFjmqGmIY/Y4HV4d3Gp2irVfcrp" crossorigin="anonymous">
    <link rel="stylesheet" href="./estilos_completar.css">
    <title>maquetacionGrid_Practica01 Guillen Dil Laureano</title>

</head>

<body>

    <!-- Laureano Guillen Dil -->

    <div class="container">

        <div class="header">
        <header>

            <h1 class="i1">Ejemplo de maquetacion con grid</h1>
            <h2 class="i2">by Isabel Cayuela Perez para Diseño de Interfaces Web</h2>
        </header>
    </div>
            <div class="nav">
                <nav>

                    <ul>

                        <li>Inicio</li>
                        <li>Galeria</li>
                        <li>Productos</li>
                        <li>Clientes</li>
                        <li>Sobre Nosotros</li>
                        <li>Contacto</li>

                    </ul>

                </nav>


            </div>


            <div class="im1">
                <main>

                    <img src="./img/1.jpg" width="580px" height="490px" class="imagen1">

                    <p class="p1">Caballos en libertad, imagen tomada en el campillo a pie de la sierra de las estancias
                    </p>
                    <p class="p1">Almeria. Valerosa y Hera
                    </p>
                    <p class="p1">La sierra de las estancias es un macizo montañoso español que cruza transversalmente el norte
                    </p>
                    <p class="p1">De la provincia de almeria
                    </p>

                </main>


            </div>





            <div class="ar1">
                <article>

                    <img src="./img/2jpg.jpg" width="260px" height="490px" class="imagen2">
                    <p class="p1">Una imagen de luminosa</p>

                </article>


            </div>

        
            <div class="ar2">
                <article>
                    <img src="./img/3.jpg" width="300px" height="290px" class="imagen3">
                    <p class="p1">Una imagen de valerosa,quiron y rucha</p>
    
                </article>
    
                </div>

                <div class="ar3">


                    <article>
                        <img src="./img/4.jpg" width="300px" height="290px" class="imagen4">
                        <p class="p1">Una imagen de favorito</p>
        
                    </article>
        
                </div>

                <div class="ar4">


                    <article>
        
                        <img src="./img/5.jpg" width="300px" height="290px" class="imagen5">
                        <p class="p1">Una imagen de valerosa y hera</p>
        
                    </article>
        
                </div>


       
             <div class="address">

                <address class="p1"> 
                    Laureano Guillen Dil
                </address>

            </div>   
            
            <div class="copyright"> 

                  <p class="p1">Todas las fotos realizadas por Isabel Cayuela Perez bajo la licencia CC B-Y-SA</p>

            </div>
            <div class="social"> 
            
                <i class="fab fa-snapchat-square"></i>
                <i class="fab fa-facebook"></i>
                <i class="fab fa-twitter"></i>
            
 
            </div>

        
    </div>


</body>

</html>
~~~

*Agrego el archivo css con el siguiente codigo:*

~~~
@import url('https://fonts.googleapis.com/css2?family=Langar&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Andika+New+Basic&display=swap');



* {

  margin: 0;



}

body{


  font-size: 16px;

}

.container {

  width: 80%;
  text-align: center;
  display: grid;
  grid-gap:0.0625em;
  grid-template-columns: minmax(6.25em,18.75em) 1fr minmax(6.25rem,12.5rem);
  grid-template-areas: "header header header"
                        "nav  im1 ar1"
                         "ar2 ar3 ar4"
                         "address copyright social ";

                      





}

.i1 {


  width: 100%;

  max-width: 625em;

  color: aquamarine;

  font-family: 'Langar', cursive;

}

.i2 {

  width: 100%;

  max-width: 625em;

  color: blue;

  font-family: 'Andika New Basic', sans-serif;

}


header {

  width: 100%;
  max-width: 62.5em;

  padding-bottom: 83px;
  padding-left: 190px;
}

.p1{

 color:aquamarine;



}

i{

font-size:1.875em;

}



.nav nav ul{


  list-style: none;


}


.content_wrapper {


  box-sizing: border-box;

}




.articles{


  box-sizing: border-box;
  




}





footer{

  box-sizing: border-box;
  

  


}

.address{

  grid-area: "address";

  grid-column-start: 1;
  grid-column-end: 1;

  width: 100%;

  padding-top: 1.875em;


  

}

.copyright{

  grid-area: "copyright";

  grid-column-start: 2;
  grid-column-end: 2;

  width: 100%;

  padding-top: 1.875em;





}

.social{

  grid-area: "copyright";

  grid-column-start: 3;
  grid-column-end: 3;

  width: 100%;

  padding-top: 1.875em;
  


}


.header{

  grid-column-start: header;
  grid-column-end: header;
  
}


.nav{

  grid-area: "nav";

  grid-column-start: 1;
  grid-column-end: 1;

  width: 100%;
  max-width: 62.5em;
  padding-top: 1.875em;
 

}

li{

 padding-bottom: 1.875em;


}



.im1{

  grid-area: "im1" ;

  grid-column-start: 2;
  grid-column-end: 2;
  width: 100%;
  max-width: 62.5em;
  padding-top: 1.875em;



}

.ar1{

  grid-area: "ar1";

  grid-column-start: 3;
  grid-column-end: 3;
  width: 100%;
  max-width: 62.5em;
  padding-top: 1.875em;


}


.ar2{

  grid-area: "ar2";

  grid-column-start: 1;
  grid-column-end: 1;
  width: 100%;
  max-width: 62.5em;
  position: relative;

  left: 15.25em;
  padding-top: 1.875em;


}

.ar3{

  grid-area: "ar3";

  grid-column-start: 2;
  grid-column-end: 2;
  width: 100%;
  max-width: 62.5em;
  position: relative;

  left: 7.75em;
  padding-top: 1.875em;
 


}

.ar4{

  grid-area: "ar4";

  grid-column-start: 3;
  grid-column-end: 3;
  width: 100%;
  max-width: 62.5em;
  padding-top: 1.875em;


}








/*  Ajustando  */


@media (max-width:1200px){

body{

  font-size: 14px;
}


.imagen1{

  width: 320px;
  height: 240px;
}

.imagen2{

  width: 160px;
  height: 240px;


}

.imagen3{


  width: 180px;


}
.imagen4{

  width: 180px;

  
}

.imagen5{

  width: 180px;

  
}


}

@media (max-width:992px){


  body{

    font-size: 13px;
  }
  
  
  .imagen1{
  
    width: 320px;
    height: 240px;
  }
  
  .imagen2{
  
    width: 160;
    height: 240px;
  
  
  }

  .im1{

          padding-right: 50px;

  }

  .header{

     font-size: 11px;


  }


  .imagen3{


    width: 90px;
    height: 80px;
  
  
  }
  .imagen4{
  
    width: 90px;
    height: 80px;
  
    
  }
  
  .imagen5{
  
    width: 90px;
    height: 80px;
  
    
  }

  

 


}


@media (max-width:768px){


  body{

    font-size: 9px;
  }
  
  
  .imagen1{
  
    width: 220px;
    height: 190px;
  }
  
  .imagen2{
  
    width: 90px;
    height: 190px;
  
  
  }

  .im1{

          padding-right: 50px;

  }


 

  .header{

     font-size: 6px;


      grid-column-start: 1;
      grid-column-end: 3;
    


  }


  .imagen3{


    width: 90px;
    height: 80px;
  
  
  }
  .imagen4{
  
    width: 90px;
    height: 80px;
    padding-left: 3.975em;
  
    
  }
  
  .imagen5{
  
    width: 90px;
    height: 80px;
  
    
  }

}

~~~

### Visualizacion

![](https://github.com/Laureano93/Practica-Con-Grid/blob/Capture/Capture.png?raw=true)

#### Enlaces
[Enlace Del Proyecto](https://github.com/Laureano93/Practica-Con-Grid/tree/main)

##### Licencia
[![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/)

