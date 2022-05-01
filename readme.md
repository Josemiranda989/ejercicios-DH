//* CLASE 3 - Introducción a Node.js y JavaScript

//? Introducción a Node.js
/*  
1 Node.js es...
un entorno de ejecución para JavaScript.

2 ¿Cuál de los siguientes comandos nos devuelve la versión de Node.js que tenemos instalada?
la primera y la tercera son correctas (node -v y node --version)

3 Para ejecutar el código de un archivo JavaScript tenemos que escribir en la terminal...
node seguido del nombre del archivo que queremos testear
*/

//? Sistema de módulos

/* Importar módulos
const moduloNativo = require('http');
const moduloInstalado = require('axios');
const moduloPropio = require('./miFuncion')
*/

/* Exportar módulos
let arrayDePeliculas = ["Harry Potter","Her", "Up", "Lego"];
module.exports = arrayDePeliculas;
*/
//* CLASE 4 - Repaso de funciones, condicionales y arrays

//? Variables

/* Declarando variables
var edad ='';
var peso ='';
*/

/* Asignando valores a las variables
var edad = 18;
var peso = 60;
*/

/* La diferencia entre var y let 
let nombre;
let apellido;
let edad;
let telefono;
let sabeProgramar;
*/

/* Las constantes
const EDAD_MINIMA = 18
const EDAD_MAXIMA = 99
*/

//? Tipos de datos

/* Una variable de cada tipo
let verdadero = true;
let nada = null;
let texto = "hola";
let numero = 1;
*/

/* Usando Number()
let positivo = Number("1")
let negativo =Number("-1")
let decimal =Number("0.1")
*/

/* Usando parseInt() 
const nan = parseInt("hola")
const correcto = parseInt(1.1234)
console.log(nan);
console.log(correcto);
*/

//? Operadores

/* Operando
let primerNumero = 1;
let segundoNumero = 2;

let resultadoSuma = primerNumero + segundoNumero;
let resultadoResta = primerNumero - segundoNumero;
let resultadoMultiplicacion = primerNumero * segundoNumero;
let resultadoDivision = primerNumero / segundoNumero;

*/

//? Funciones

/* Declarar funciones 
function ejemplo (saludo) {
    return "hola, soy una función"
}
*/

/* Declarando funciones en variables
let ejemplo = function saludar () {
    return "hola, soy una función expresada"
}
*/

/* Funciones con parámetros
function saludar(nombre, apellido) {
    return 'Hola, ' + nombre + ' ' + apellido + '!';
}
*/

/* Numeros pares
function esPar (n) {
    return n % 2 == 0 
}
*/

/* Declarando tres funciones
function anterior (n) {
    return n -1  
    }

function triple (n) {
    return n * 3
}

function anteriorDelTriple(n){
  let resultado;
  resultado = triple(n);
  resultado = anterior(resultado);
  return resultado;
}
*/

//? Condicionales

/* Mi primer if
let dato = true;

if (dato == true) {
    console.log ("es true")
} else console.log ("es false")
*/

/* igualdad, if y else
let lenguaje = "javascript";
if ( lenguaje == "javascript" ) {
    console.log ("Estoy aprendiendo")
} else ( console.log ("Lo aprenderé más adelante"))
*/

/* ¿Puede pasar cosme fulanito?
function puedePasar(nombre) {
    if ( nombre == "Cosme Fulanito" ) {
        return false
    } else return true
}
*/

//? Arrays

/* 
1 Un array permite: 
Ambas opciones son correctas (generar una coleccion de datos ordenados y almacenar distintos tipos de datos)

2 El primer índice de un array es siempre:
0

3 Para indicar el inicio y el fin de un array usamos:
Corchetes []
*/

//? Métodos de Arrays

/* indexOf
let alumnos = ["Juan", "Pepe", "Jorge", "Francisco"]
let indiceJuan = alumnos.indexOf("Juan")
let indiceFrancisco = alumnos.indexOf("Francisco")
*/

/* Join
let arrayFrase = [
  "No",
  "he",
  "fracasado,",
  "simplemente",
  "me",
  "he",
  "topado",
  "con",
  "diez",
  "mil",
  "soluciones",
  "equivocadas"
];

let fraseNueva = arrayFrase.join(" ")
console.log (fraseNueva)
*/

/* Pop
let estudiantes = [
  {
    nombre: "Alvaro",
    promedio: 9,
    curso: "Android"
  },
  {
    nombre: "Daniel",
    promedio: 6,
    curso: "Full Stack"
  },
  {
    nombre: "Alexis",
    promedio: 3,
    curso: "iOS"
  }
];

let alumnoEgresado = estudiantes.pop(2)
*/

/* Push
let estudiantes = [
  {
    nombre: 'Alvaro',
    promedio : 9,
    curso : 'Android',
  },
  {
    nombre: 'Daniel',
    promedio : 6,
    curso : 'Full Stack',
  },
  {
    nombre: 'Alexis',
    promedio : 3,
    curso : 'iOS',
  },
]
let juan = {
  nombre: "Juan",
promedio: 5,
curso: "iOS",
}
estudiantes.push(juan)
let miguel = {
  nombre: "Miguel",
promedio: 2,
curso: "Android",
}
estudiantes.push(miguel)
*/

/* Shift
 let estudiantes = [
 {
    nombre: 'Alvaro',
    promedio : 9,
    curso : 'Android',
  },
   {
     nombre: 'Daniel',
     promedio : 6,
     curso : 'Full Stack',
   },
   {
     nombre: 'Alexis',
     promedio : 3,
     curso : 'iOS',
   },
 ]

let alumnoDeBaja = estudiantes.shift()
*/

/* Unshift
let estudiantes = [
  {
    nombre: 'Alvaro',
    promedio : 9,
    curso : 'Android',
  },
  {
    nombre: 'Daniel',
    promedio : 6,
    curso : 'Full Stack',
  },
  {
    nombre: 'Alexis',
    promedio : 3,
    curso : 'iOS',
  }
]
let mariana = {nombre: "Mariana",

promedio: 9,

curso: "Full Stack"}
estudiantes.unshift(mariana)
let Francisco = {nombre: "Francisco",

promedio: 2,

curso: "Android"}
estudiantes.unshift(Francisco)
*/


//* CLASE 5 - JSON, más condicionales y ciclos

//? JSON

/*  
1 ¿Qué significan las siglas JSON? 
JavaScript Object Notation.

2 ¿Para qué se utiliza JSON?
Comunicar sistemas entre sí.

3 ¿Para qué puedo utilizar el método JSON.stringify()?
Para transformar un objeto en un string.

4 ¿Para qué puedo utilizar el método JSON.parse()?
Para transformar un string en un objeto.
*/

//? Métodos de Strings

/* Completar URL
function dominio ( nombreDominio )
{
  return "http://www."+nombreDominio;
}
console.log(dominio("digitalhouse.com.ar"));
console.log(dominio("pokemon.com.ar"));
*/

/* Contar los caracteres
let texto = "Hola mundo";
console.log(texto.length)
*/

/* Reemplazo fast fast
function reemplazoFastFast (texto, vieja, nueva ) {
    return texto.replace(vieja, nueva)
}
*/

/* ¿Están hablando de mí?
function menciona (texto, palabra) {
if (texto.indexOf(palabra) == -1) {
    return false
} else {
    return true 
    }
}
*/

/* Solo el nombre
let frase = 'Hola!, soy Carli';
let licenciada = frase.slice(11)
 */


//? Objetos literales

/*  
1 Un objeto literal puede tener...
la cantidad de propiedades que queramos.

2 Las propiedades de un objeto literal pueden almacenar...
cualquier tipo de dato.

3 Seleccionar la sintaxis correcta para ejecutar el método de un objeto.
objeto.metodo()

4 Para separar las propiedades dentro de un objeto literal....
usamos el carácter coma ","

5 Cuando usamos una función constructora de objetos, definimos...
generar un "molde" para crear la cantidad de objetos que deseemos.
*/

/* 
Crear un objeto literal
let perro = {
    nombre : "perla",
    edad : 2,
    vacunado : true
}
*/

/* 
Utilizando los métodos de los objetos
let deportista = {
    energia: 100,
    experiencia: 10,
    nombre: "Aimar",
    entrenarHoras: function (horas) {
      this.horas = horas;
      this.energia = this.energia - (this.horas*5);
      this.experiencia = this.experiencia + (this.horas*2)
    }
};

console.log("==Antes de comenzar entrenamiento==");
console.log("Deportista energia: "+deportista.energia);
console.log("Deportista experiencia: "+deportista.experiencia);
console.log("==ENTRENANDO==");
deportista.entrenarHoras(5);
console.log("==FIN ENTRENAMIENTO==");
console.log("Deportista energia: "+deportista.energia);
console.log("Deportista experiencia: "+deportista.experiencia);
*/

//? Arrow Functions

/* Convertir a arrow function
let dameCinco = () => {
  return [1,2,3,4,5] ;
}
let multiplicarPorDos = () => {
  return 123 * 2;
}
let mostrarNombre = () => "Mi nombre es Hernán";
*/

/* Arrow function con parámetro
let saludar = nombre => 
'Hola, ' + nombre + '!';
*/

/* Ahora probemos con más de uno
let saludar = (nombre, apellido) => {
  return  'Hola, ' + nombre + ' ' +  apellido + '!';
}
*/

//? Condicionales

/* Fin de semana
let dia = 'jueves'
function finDeSemana (dia) {
switch (dia) {	
    case 'viernes' :
        console.log('buen finde');
        break;
    case 'lunes' :
        console.log('buena semana');
        break;
    default:
        console.log('buen dia');
    }
}
*/

/* Tengo clases
function tengoClases(dia) {
    switch (dia) {
        case "lunes":
            console.log("tenés clases");

        case "miércoles":
            console.log("tenés clases");

        case "viernes":
            console.log("tenés clases");
            break;
        default:
            console.log("no tenés clases");
    }
}
*/

/* Practicando el if ternario
let bicicletaA = {
    rodado: 18,
    marca: "Mountain Bike"
}
let bicicletaB = {
    rodado: 24,
    marca: "Aurora"
}

let bicicletaConRodadoGrande = bicicletaA > bicicletaB ? bicicletaA  :  bicicletaB;

console.log("La bicicleta con  mayor rodado es la "+ bicicletaConRodadoGrande.marca );
*/

//? Ciclos: repaso del for

/* Repetir como un loro
function loro (texto) {
    for (let i=0; i<5;i++) {
        console.log(texto)
    }
}
*/

/* Contar impares 
function noParesDeContarImparesHasta(numero){
    let impares = 0
   for (let i =0; i <= numero; i++ ) {
       if (i % 2 != 0) {  
           impares++
      }
   }
   return impares
}

console.log(noParesDeContarImparesHasta(4))
*/

//* CLASE 6 - Callbacks, más ciclos y nuevos métodos

//? Callbacks

/* Pasar un callback
function doble (num) {
    return num *2
};

function triple (num) {
    return num *3
};

function aplicarCallback (num, funcion) {
    return funcion(num)
}
*/

/* Hagamos una calculadora
let suma = (num1,num2) => num1 + num2
let resta = (num1,num2) => num1 - num2
let division = (num1,num2) => num1 / num2
let multiplicacion = (num1,num2) => num1 * num2

function calculadora (num1,num2, operacion) {
    return operacion(num1,num2)
}
*/

/* Pasar un callback reloaded
function agregarHttp(url) {
    return "http://" + url
}

function procesar(url,funcion){
    let array = []
    for (let i = 0; i <= url.length; i++) {
        array.push(funcion(url[i]))
    }  
    return array
}
*/



//? Métodos de arrays 2

/* Filter con números
let estudiantes = [
    {nombre: 'John', promedio: 8.5, aprobado: true},
    {nombre: 'Jane', promedio: 7, aprobado: true},
    {nombre: 'June', promedio: 3, aprobado: false},
]

let aprobados = estudiantes.filter(function(estudiantes){
    return estudiantes.aprobado === true
})

let desaprobados = estudiantes.filter(function(estudiantes){
    return estudiantes.aprobado === false
})
*/

/* map ()
let horariosPartida = [12, 14, 18, 21];

let horariosAtrasados = horariosPartida.map(function(hora) {
    return hora - 1
})
*/

/* reduce()
let vueltas = [5, 8, 12, 3, 22]

let totalVueltas = vueltas.reduce(function(acum,numero) {
    return acum + numero
})
*/

/* forEach
let listaDeSuperMercado = [
    'Bife de chorizo', 
    'Coca Cola', 
    'Bananas', 
    'Lechuga', 
    'Chimichurri', 
    'Lata de tomates', 
    'Arvejas', 
    'Cereales', 
    'Pechuga de pollo', 
    'Leche'
];

listaDeSuperMercado.forEach(function(valor,indice) {
    console.log(valor)
})
*/

//? Objeto Date

/* Date
let dia = fecha.getDate()
let mes = fecha.getMonth()
let anio = fecha.getFullYear()

console.log("Día: "+fecha.getDate());
console.log('Hoy es el día '+dia+' del mes '+(mes)+' del año '+anio);
*/

//? Destructuring

/* Destructuring
let destinosDelMundo = ['Marruecos', 'Bariloche', 'Barcelona', 'China', 'Grecia']
let [,bariloche,,china,] = destinosDelMundo
*/

/* Destructurando objetos
let auto  = {marca: 'Ferrari', kilometros: 31, color: "Rojo"};
let { marca,   color} = auto;*/

//? Spread operator y rest parameter

/* 
1 El operador spread nos sirve para:
copiar y mover datos de un lugar a otro.

2 Podemos usar el operador spread...
sobre cualquier elemento iterable.

3 ¿Podemos usar el operador spread para definir funciones?
Sí, pero en ese contexto lo llamamos parámetro rest.

4 Implementando el parámetro rest podemos:
definir una función que acepte cualquier número de argumentos.

5 El parámetro rest se escribe:
siemre al final
*/

//? Cierre de módulo

/* Pensar la pregunta
Juan menciona sus tres ideas para que lo ayudes a elegir la correcta. ¿Cuál de las siguientes ideas te parece la más correcta para representar un auto?
-Un objeto literal con las propiedades de cada auto. */

/* Aprobando la propuesta de Juan
Juan pensó también en opciones para representar la lista. Las presentó de la siguiente manera en código. ¿Podrías ayudarlo una vez más a elegir la que te parezca correcta?
-let autos = [ { }, { }, { } ]; */

/* Ayudando a Juan
 Ahora que tenemos guardada la lista de vehículos, Juan se pregunta cómo hará el sistema para usar esa información dentro de diferentes archivos. -María te consulta cuál sería la manera correcta de resolver la duda de Juan.
-Exportando el contenido de la variable mediante "module.exports" y requiriéndolo en los archivos que lo necesiten. */


/* ¡Al fin es momento de codear!
let autos = [ 
    {
        marca : "Ford",
        modelo:  "Fiesta",
        precio: 150000,
        km: 200,
         color:  "Azul",
          cuotas: 12,
           anio: 2019,
            patente: "APL123",
             vendido: false,
    },
    {
        marca : "Toyota",
        modelo: "Corolla",
        precio: 100000,
        km: 0,
         color: "Blanco",
          cuotas: 14 ,
           anio: 2019,
            patente: "JJK116",
             vendido: false,
    }
]

module.exports = autos
*/

/* El proyecto sigue avanzando
A la semana, el proyecto avanza y María nos pide otro requerimiento, esta vez un poco más avanzado. Nos comenta que la concesionaria ahora necesita poder buscar los automóviles por patente y venderlos. Para esto, María nos encargó pensar la forma en que representaremos a la concesionaria.
Al terminar la reunión, Juan se acerca para comentarte tres ideas que tuvo. María, a unos metros, escuchó las opciones y te encargó definir cuál será la más eficaz.
- Podríamos tener un objeto literal que represente a la concesionaria con los autos que creamos y que esta tenga las funcionalidades de buscar por patente y marcar como vendido un auto.
*/

/* Concesionaria completa
const autos = require("./autos");
let concesionaria = {
  autos: autos,
  buscarAuto: function (patente) {
    for (let i = 0; i < autos.length; i++) {
      if (autos[i].patente == patente) {
        return autos[i];
      }
    }
    return null;
  },
  venderAuto: function (patente) {
    const auto = this.buscarAuto(patente);
    if (auto) {
      auto.vendido = true;
    }
  },
  autosParaLaVenta: function () {
        //   return autos.filter(auto => auto.vendido == false)
    return this.autos.filter(function (auto) {
      return auto.vendido == false;
    });
  },
  autosNuevos: function () {
    let autosVenta = this.autosParaLaVenta();
        //   return autosVenta.filter(auto => auto.km <100)
    return autosVenta.filter(function (auto) {
      return auto.km < 100;
    });
  },
  listaDeVentas: function () {
    let precios = [];
    for (let i = 0; i < this.autos.length; i++) {
      if (this.autos[i].vendido == true) {
        precios.push(this.autos[i].precio);
      }
    }
    return precios;
  },
  totalDeVentas: function () {
//           let resultado = this.listaDeVentas().reduce((a,b) =>
//     a + b, 0)
//    return resultado}
    let resultado = this.listaDeVentas().reduce(function (a, b) {
      return a + b;
    }, 0);
    return resultado;
  },
  puedeComprar: function (auto, persona) {
    if (
      auto.precio <= persona.capacidadDePagoTotal &&
      auto.precio / auto.cuotas <= persona.capacidadDePagoEnCuotas
    ) {
      return true;
    } else return false;
  },
  autosQuePuedeComprar: function (persona) {
    let puedeComprar = [];

    this.autosParaLaVenta().forEach((item) => {
      if (this.puedeComprar(item, persona) == true) {
        puedeComprar.push(item);
      }
    });
    return puedeComprar;
  },
};
*/




//* CLASE 7 - Manejo de Proyectos con Git

//? Introduccion a git

/*  
4 Git es
un software

5 Git me permite desarrollar un proyecto con control de versiones en...
la nube con servicios como Github

6 ¿Git permite mantener un historial de cómo fue cambiando el proyecto?
si
*/

//? Github

/* 
1 Git y Github
Git es un sistema de versionado y GitHub un sistema en la nube que provee de ese servicio.

2 Un repositorio en GitHub es…
un proyecto en la nube utilizando Git como sistema de versionado

3 ¿Cuál es la diferencia entre un repositorio local o remoto?
Un repositorio local es el que se encuentra en mi computadora y el remoto es el de GitHub.
*/

//? Creando nuestro primer repositorio local

/* 
1 ¿Con qué comando creo mi repositorio local?
git init
*/

//? Agregando archivos al repositorio

/* 
1 ¿Cómo guardo los cambios en Git en forma versionada?
Commits

2 ¿Cómo agrego los archivos a Git?
git add

3 Si tengo el archivo productos.js y lo agrego a Git mediante el comando git add y posteriormente lo modifican...
Hay que volver a agregarlo al commit con otro git add
*/

//? Confirmando archivos

/* 
1 Un commit tiene...
Fecha autor y mensaje

2 Con git
podemos tener un orden cronológico del proyecto.
podemos revertir cambios y volver a un estado anterior.

3 Seleccionar el orden correcto para persistir los cambios de productos.js.
git add productos.js —> se modifica el archivo —> git add productos.js —>git commit -m "Carrito agregado"
*/

//? Subiendo archivos

/* 
1 ¿Con qué comando envío los archivos de mi repositorio a GitHub?
git push

2 En Git, ¿qué es una rama?
Es una línea paralela para agregar funcionalidades sin afectar a la rama principal.

3 Para git...
el repositorio remoto se llama "origin"
*/

//? Bajando archivos

/* 
1 ¿Cómo descargás por primera vez un repositorio?
git clone "url del repositorio"

2 ¿Cómo actualizás el código en tu repositorio local?
git pull origin master
*/

//? Hacia la clase en vivo

/* 
1 ¿Para qué queremos un sistema de versionado de archivos?
para conocer que archivos fueron creados y que modificaciones tuvieron por parte de los usuarios con fecha y hora.

2 ¿Qué diferencias hay entre Git y GitHub?
Git es un sistema de versionado y GitHub un sistema en la nube que provee de ese servicio.
*/


//* CLASE 8 - Scrum

//? ¿Qué pasaba antes de las metodologías ágiles?

/*  
    1 ¿En qué momento se empieza a hacer popular la metodología de cascada?
A partir de 1985 cuando el departamento de defensa de EEUU las declara requisito para cualquier contratista.

2 ¿En qué casos funciona bien la metodología de cascada?
    a + b

3 ¿Cuáles son las debilidades de la metodología de cascada?
a+b+c+d      
*/

//* CLASE 10 - Anatomía de un sitio web

//? Introducción a Servidores

/*  
    1 En la arquitectura cliente-servidor...
El cliente genera el request y el servidor devuelve un response.

2 ¿Qué es un web server?
Programa del servidor que procesa peticiones y envía respuestas.

3 ¿Cuál de los siguientes lenguajes y/o componentes puede pertenecer al front-end? (Podés marcar más de una respuesta)
HTML, JAVASCRIPT, CSS

4 ¿Cuál de los siguientes lenguajes y/o componentes puede pertenecer al back-end? (Podés marcar más de una respuesta)
PHP, BASE DE DATOS, JAVASCRIPT
*/

//? Introducción a HTTP

/* 
1 HTTP es
un protocolo de transferencia

2 HTTP nos permite...
transferir informacion en la web

3 Utilizando el método GET podemos...
podemos enviar información al servidor y también recibirla.

4 El método POST es más seguro que el método GET cuando se trata de enviar información al servidor.
Verdadero

5 En HTTP, cuando hablamos de request nos referimos al...
Cliente

6 En HTTP, cuando hablamos de response nos referimos al...
Servidor

7 ¿Cuáles de los siguientes métodos son los más utilizados por HTTP?
get, patch, post, put, delete
*/

//? Introducción a Express

/* 
1 ¿Qué es un framework?
Es una librería de código con funcionalidades armadas para usar.

2 Express sirve para...
desarrollar una aplicación web en forma más sencilla y eficiente.

3 Por convención, ¿qué objeto utilizaremos para acceder a toda la funcionalidad de Express?
app
*/

//? Servidor web con Express

/* Instanciar servidor
const express = require('express');
const app = express();

app.listen(8000, () =>
console.log ("Levantando un servidor con Express"))
*/

//? Routing & Response

/* Ruta GET home
const express = require('express');
const app = express();

app.get ('/home', function (req,res) {
    res.send ("Hola, estamos en el home")
})
*/

/* Ruta GET perfil
const express = require('express');
const app = express();
let saludo = "Bienvenido/a, ahora estamos en tu perfil"
app.get ('/perfil', function (req,res) {
    res.send (saludo)
})
*/

/* Ruta GET agregar producto
const express = require('express');
const app = express();
let producto = {
    tipoProducto : null,
    precio : null,
    cantidad : null
}
app.get ('/producto/agregar', function (req,res) {
    res.send (producto)
})*/

//? Estructura de carpetas y Send file

/* About us
const path = require('path');
app.get('/about-us', (req, res) => {
    res.sendFile( path.join(__dirname, '/views/about-us.html'))
});
 */

//? Hacia la clase en vivo
/* 
const express = require ('express')
const app = express()
const path = require('path')

app.listen(3000, () => {
    console.log("servidor corriendo")
})

app.get('/', function(req,res){
    res.sendFile(path.join(__dirname, '/views/home.html'))})

app.get('/404', function(req,res){
    res.send("Error página no encontrada")})
*/

//* CLASE 11 - Creando la estructura de un sitio web


//? Introduccion a HTML
/*  
1 ¿Qué significa HTML?
HyperText Markup Language

2 Cuando escribimos un archivo HTML, podemos decir que luego:
el navegador procesa ese código HTML y lo muestra al usuario.
*/

//? Etiquetas y atributos

/* Mi primer HTML
<html>
    <head>
        <title>Mi primer HTML</title>
    </head>
    <body>
        Soy el body
    </body>
</html>
*/

//? Elementos de linea y de bloque

/* Ejercitación
<html>
<head>
</head>
<body>
    <span>Las próximas lineas de texto debe estar cada una contenida dentro de una etiqueta span </span>
    <span>Esto es un texto dentro de un span.</span>
    <span>Otro texto dentro de un span</span>
    <span>Ultimo texto dentro de un span.</span>
    <div> 
    Las próximas lineas de texto debe estar cada una contenida dentro de una etiqueta div 
    </div>
    <div>Esto es un texto dentro de un div.</div>
    <div>Otro texto dentro de un div.</div>
    <div>Ultimo texto dentro de un div.</div>
  </body>
</html>
*/

//? Etiquetas de Texto

/* Practicamos como escribir etiquetas de texto
<html>
    <head>
        <title>Etiquetas de texto</title>
    </head>
    <body>
        <h1>Holaaaa</h1>
        <h2>Como estan</h2>
        <p>lorem15</p>
    </body>
</html>
*/

//? Listas

/* Armando listas
<html>
    <head>
        <title>Listas</title>
    </head>
    <body>
        <ul>
            <li> blanco </li>
            <li> verde </li>
            <li> azul </li>
        </ul>
        <ol start="10">
            <li> ironman1 </li>
            <li> ironman2 </li>
            <li> ironman3 </li>
        </ol>
    </body>
</html>
 */

//? Rutas, hipervínculos e imágenes

/* Mis primeras rutas
<html>
    <head>
        <title>Rutas</title>
    </head>
    <body>
        <a href="https://www.digitalhouse.com">Digital House</a>
        <img src="http://bit.do/imagen-blend" >
    </body>
    </html>
*/

/* Imagenes linkeadas
<html>
    <head>
        <title>Imágenes Linkeadas</title>
    </head>
    <body>
        <a href="https://google.com">
            <img src="https://bit.ly/2WDMapV">
        </a>
    </body>
</html>
*/

/* Listas linkeadas
<html>
    <head>
        <title>Listas linkeadas</title>
    </head>
    <body>
        <ul>
            <li>
                <a href="https://www.facebook.com">Facebook</a>
            </li>
            <li>
                <a href="https://www.instagram.com">Instagram</a>
            </li>
            <li>
                <a href="https://www.ole.com.ar">Olé</a>
            </li>
        </ul>
    </body>
</html>
*/

//? Introduccion a la semántica

/* 
1 Las etiquetas header, nav, footer, section, article son de tipo:
Bloque

2 La etiqueta ________ nos permite definir una pieza de contenido independiente.
article

3 La etiqueta ________ nos permite definir una sección de contenido.
section
*/

//? Estructura de un sitio web

/* 
¿Cuáles de los siguientes bloques forman parte de los principales?
Footer, Header, Section
*/

//* CLASE 12 - Agregando estilos

//? Introduccion a CSS

/*  
1  ¿Cómo se escribe un selector de etiqueta?
etiqueta{}

2 ¿Cómo se escribe un selector de clase?
.clase{}

3 ¿Cómo se escribe un selector de id?
#id{}

4 ¿A qué elemento afecta el siguiente selector? p#unico{}
A una etiqueta <p> con id "unico".

5 ¿A qué elemento afecta el siguiente selector? ul li.rojo{}
A la etiqueta <li> con clase "rojo" que sea hija de una etiqueta <ul>.

6 ¿A qué elemento afecta el siguiente selector? ol#negro li
A toda etiqueta <li> que sea hija de una etiqueta <ol> con id "negro".
*/

/* Primer selector\
p{
  color:red
}
*/

/* Más selectores
h3{
  color:blue
}

.negrita{
  font-weight: bold
}

#gigante{
  font-size: 40px
}
*/

/* Atributo class 
.destacado {
    color: gold;
}

.en-mayuscula {
    text-transform: uppercase;
}

#whatsapp {
    background-color: green;
    color: white;
}
*/

/* Incluyendo un archivo css 
<html>
  <head>
    <title>CSS</title>
    <link href="https://bit.do/blend-css" rel="stylesheet">
  </head>
    
  <body>
     <div class="container">
       <div class="jumbotron">
         <h1>¡Hola Mundo!</h1>
         <button class="btn btn-default">Continuar</button>
       </div>
     </div>
  </body>
</html>
*/

//? Fuentes

/* Agregando estilos
p {
    font-family: Arial;
    font-size: 20px;
    font-weight: bold;
    font-style: italic;  
    text-decoration:underline;
    text-align: center;
}
*/

//? Fondos

/* Imagen de fondo
body {
    background-image: url('https://images3.alphacoders.com/621/621682.jpg');
    background-size: cover;
} 
h1 {
    color: #f4e033;
    background-color: rgba(0,0,0,0.8);
    }

h2 {
    background-color: orange;
    color: white;
    opacity: 0.4

}
*/


//* CLASE 13 - Diseño Adaptativo

//? Modelo de caja

/*  Modelando Cajas
div {
            width: 100px;
            padding: 5px;
            border: solid 1px red;
            margin: 10px;
            box-sizing: border-box;
}
*/

/* Estilizando el sitio
header {
                background-color: lightseagreen;
                color: white;
                font-size: 28px;
                border-bottom: solid 3px indigo;
                padding: 22px;
                margin-bottom: 15px;
                text-align:center;
                box-sizing: border-box

}
section {
                width: 50%;
                margin-left: 25%;
                background-color: gainsboro;
                margin-bottom: 15px;
                padding-left: 12px;
                padding-top:30px;
                padding-bottom:30px;
                border: dashed 1px black;
                border-radius: 5px;
                text-align: center;
                box-sizing: border-box                
}
footer {
            background-color: rebeccapurple;
            color:white;
            border-top: solid 1px lightseagreen;
            padding: 12px;
            height: 40px;
            text-align: center;
            box-sizing: border-box            
}
*/

//? Viewports

/*  Adaptando el sitio a múltiples dispositivos
<html>
  <head>
    <title>Viewport</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
  </head>
  <body>
    <marquee>¡Primeros pasos en el diseño web responsive!</marquee>
  </body>
</html>
*/

//? Medidas relativas

/*   Jugando con vh y vw
.arriba {
background-color: blueviolet;
height: 40vh;
width: 100%;
}
.abajo {
  height: 60vh;
  width: 100%;
background-color: brown;
}
*/

//? Media queries

/*  
1 ¿Qué hacemos cuando escribimos nuestras reglas de CSS mobile-first?
Primero escribimos reglas de CSS en el ámbito global para teléfonos móviles y luego hacemos reglas más específicas dentro de media queries.

2 ¿Para que sirven las media queries?
Para definir reglas de CSS que se apliquen en algunos viewport, pero no en otros.

3 ¿Qué hace la siguiente media query? @media(min-device-width: 320px) and (max-device-width: 480px)
Las reglas de CSS que escribamos adentro solo aplicarán si el viewport tiene entre 320px y 480px de ancho.
*/

//* CLASE 14 - Posicionamiento avanzado con flexbox

//? Introduccion a flexbox

/*  
1 Que es flexbox
una metodologia de css

2 utilizando flexbox
disponemos de una gran libertad para manipular los elementos dispuestos en el HTML.
*/

//? Ejes

/* Reordenando un texto
.frase-cortazar {
  display:flex;
  flex-direction: column-reverse
}
*/

/* Reordenando otra frase
.frase {
  display: flex;
  width: 350px;
  flex-direction: row-reverse
}
*/

/* Estilizando elementos de forma horizontal
.nav-bar {
  display:flex;
    justify-content: space-around
}
.enlaces {
  display:flex;
}
*/

/* Centrando la x
.juego-dardos {
display: flex;
justify-content: center;
align-items: center;
}
*/

//? Estructura básica

/* Disponiendo UL's
.nav-bar {
    display:flex
}
*/

/* Respetando medidas en el contenedor
.contenedor {
display:flex;
flex-wrap: wrap
}
*/

//? Items

/* Ordenando la evolución de Homero
.homero-sapiens {
  display: flex;
  width: 50%;
}
.sapiens-5 {
    order:1
}
*/

/* Ordenando imágenes
.surf-en-el-mar {
  display: flex;
  width: 100%;
}
.tabla {
  order:-1
}
*/

/* Situando elementos al final
.tetris {
  display: flex;
}
.pieza-tetris {
 align-self: flex-end
}
*/

//* CLASE 15 - Trabajando con Formularios

//? Formularios

/*  Primer formulario
<html>
  <head>
    <title>Primer formulario</title>
  </head>
  <body>
    <form action="resultado.html" method="POST">    
    </form>
  </body>
</html>
*/

/* Campos de texto
<html>
<head>
    <title>Campos en el formulario</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <label for="nombre">Ingrese su nombre:</label>
      <input type="text" name="nombre" id="nombre">
    </form>
  </body>
</html>
*/

/* Más campos de texto
<html>
<head>
    <title>Formulario de registro</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <p>
            <label for="nombre">Ingrese su nombre:</label>
         <input type="text" name="nombre" id="nombre">
      </p>
      <p>
        <label for="email">Email:</label>
        <input type="email" name="email" id="email">
      </p>      
      <p>
        <label for="password">Contraseña:</label>
        <input type="password" name="password" id="password">
      </p>
    </form>
  </body>
</html>
*/

/* Completar el formulario
<html>
<head>
    <title>Formulario de registro</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <p>
            <label>Nombre:</label>
        <input type="text" name="nombre" required>
      </p>
      <p>
        <label>E-mail:</label>
        <input type="email" name="email" required>
      </p>
      <p>
        <label>Contraseña:</label>
        <input type="password" name="password" required>
      </p>
      <p>
        <input type="submit" value="Enviar">
      </p>
    </form>
  </body>
</html>
*/

//? Radio button y checkboxes

/* ¿Tiene mascota? 
<html>
<head>
    <title>Formularios</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <label for="mascota">¿Tenés mascota?</label>
      <label for="mascota">Si</label>
      <input type="radio" name="mascota" value="mascota">
            <label for="mascota">No</label>
      <input type="radio" name="mascota" value="mascota">
        <input type="submit" value="Enviar">
    </form>
  </body>
</html>
*/

/* Hobbies
<html>
<head>
    <title>Formularios</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <label for="hobby"> ¿Cuáles son tus hobbies?
        <label><input type="checkbox" name="hobby" value="pescar">Pescar</label>
        <label><input type="checkbox" name="hobby" value="correr">Correr</label>
        <label><input type="checkbox" name="hobby" value="yoga">Yoga</label>
                </label>
        <input type="submit" value="Enviar">
    </form>
  </body>
</html>
 */

//? Formularios avanzados

/*  Seleccionando el mes
<html>
<head>
    <title>Formularios</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <label>Elegí el mes de tu cumpleaños</label>
        <select name="mes">
            <option value="1">Enero</option>
            <option value="2">Febrero</option>
            <option value="3">Marzo</option>
            <option value="4">Abril</option>
            <option value="5">Mayo</option>
            <option value="6">Junio</option>
            <option value="7">Julio</option>
            <option value="8">Agosto</option>
            <option value="9">Septiembre</option>
            <option value="10">Octubre</option>
            <option value="11">Noviembre</option>
            <option value="12">Diciembre</option>
        </select>
        <input type="submit" value="Enviar">
    </form>
  </body>
</html>
*/

/* Escribir comentario
<html>
<head>
    <title>Formularios</title>
</head>
<body>
    <form action="resultado.html" method="POST">
        <label>Dejanos tu comentario</label>
    <textarea></textarea>
    <button type="submit">Enviar</button>
    <button type="reset">Borrar</button>
    </form>
  </body>
</html>
*/

//? Pseudo selectores

/*  
1 ¿Cuál de las siguientes opciones es un pseudo selector escrito de manera correcta?
input:focus

2 ¿Cuál de las siguientes opciones es un pseudo selector escrito de manera correcta?
A las etiquetas p cuando se les pasa el cursor del mouse por encima.
*/

//* CLASE 16 - Organizando y animando Formularios

//? Position

/* Posicionando por primera vez
.primero {
  position: relative;
  left: 20px;
  top: 30px;
}
.segundo {
    position:absolute;
    right: 30px;
    bottom: 20px;
}
*/

/* Lindo gatito
.contenedor {
    position:relative;
}
.gorrito {
        width:120px;
        position:absolute;
        left:70px;
}
*/

/* Ubicando el navbar
.nav-bar {
  position:fixed;
  top:5px;
  width:100%;
}
*/

//? Z-index

/* Acomodando bloques
.amarillo {
  position: relative;
  top:20px;
}
.rojo {
position:relative;
z-index:10
}
*/

//? Transiciones

/* Transiciones simples con CSS
.mi-elemento {
    width: 100px;
    height: 100px;
    background-color: salmon;
    transition: border-radius 450ms;
} 
.mi-elemento:hover {
    border-radius: 50%;
}
*/

//? Animaciones

/* Animación por terminar en CSS
.mi-elemento {
  width: 200px;
    height: 200px;
    position: relative;
    border-radius: 100%;
    animation-iteration-count: infinite;
    animation-direction: alternate;
    animation-name:achicando;
     animation-duration:1000ms;
}
@keyframes achicando {
    0% {
        background-color: salmon;
    }
    
    100% {
        background-color: peachpuff;
        height: 100px;
        width: 100px;
        opacity: 0.5;
    }
}
*/

//* CLASE 19 - Patrones de diseño MVC

//? Introduccion a MVC

/*
1 ¿Que es un patrón de diseño? 
Conjunto de reglas que definen la arquitectura de un sistema.

2 MVC significa...
Model view controller

3 En el Modelo Vista Controlador...
La vista habla con el controlador y el controlador con el modelo.
*/

//? Controladores

/* 
1 ¿Qué es un controlador?
El que mantiene la lógica de negocio.

2 ¿Cuál de las siguientes frases es correcta? El controlador...
mantiene diálogo con la vista. 
mantiene diálogo con el modelo.
*/

/* Primer controller
let carritoController = {
  sacarItem: function () { },
  consultarItem: function () { },
  agregarItem: function (req, res) {
    res.send('Item Agregado');
  },
};
module.exports = carritoController
*/

/* Ruteando controladores
let express = require('express')
let router = express.Router();
let carritoController = require('../controllers/carritoController')
router.get('/:item', carritoController.agregarItem)
module.exports = router
*/

//? Rutas parametrizadas

/* Buscando series 
const express = require('express');
const app = express();
app.get('/series', function (req, res) {
    res.send(series)
})
*/

/* Buscar una serie
const express = require('express');
const app = express();
app.get('/serie/:id', (req, res) => {
    let id = req.params.id
    for (let i = 0; i < series.length; i++) {
        if (series[i].id == id) {
            res.send(series[i])
        }
    }
})
*/

//? Sistema de ruteo

/* Modularizar rutas
const express = require ('express');
const router = express.Router();
*/

/* Exportar rutas
const express = require('express');
const router = express.Router();
router.get('/', (req,res) => {
});
router.get('/:genero', (req,res) => {
});
router.get('/crear', (req,res) => {
});
module.exports = router
*/

/* Usando rutas
const express = require('express');
const app = express();
const rutasSeries = require('./routes/series')
app.use('/series', rutasSeries);
*/

//* CLASE 20 - Vistas dinámicas con EJS

//? Introducción a template engine

/*  
1 ¿Qué permite un template engine?
Que los archivos HTML sean dinámicos. Reutilizar código HTML

2 ¿Qué extensión deben tener los archivos de HTML para que EJS los procese?
.ejs
*/

//? Instalación e implementación

/*  
1 ¿Cuáles de las siguientes frases son correctas?
Puedo crear un proyecto con EJS desde cero. Puedo instalar EJS en un proyecto existente.

2 El template EJS toma por default las vistas de la carpeta...
views

3 ¿Qué método tengo que ejecutar para que mi aplicación establezca a EJS como template engine?
app.set('view engine','ejs');
*/

//? Primera vista

/* Renderizando el login
let userController = {
    loginUser: function (req,res){
        res.render("login");
    }
}
*/

//? Tags en EJS

/*  
1 ¿Qué permite la etiqueta <%?
Agregar código y estructuras de JavaScript al HTML.

2 En un archivo .ejs. ¿Dónde agregarías la etiqueta <% y %> para que se pueda ejecutar correctamente el for?
for(var i=0; i< unArray.length; i++){  
}
Una por cada línea de JavaScript. En este caso, una apertura y cierre en la primera línea y otra en la última, donde se encuentran las llaves.

3 ¿Para qué sirve la equiteta <%=?
Permite imprimir un valor dinámico.
*/

//? Parámetros compartidos

/*  Parámetros compartidos
let productos = ['Helado 1/4 kg', 'Franui Chocolate Negro', 'Surtido Chocolate 1/2kg'];
let carritoController = {
    checkout: function (req,res){
        res.render('checkout', {'items': productos});
    }
}     
*/

//? Archivos parciales

/*  
1 ¿En dónde deberiamos guardar las vistas fragmentadas de EJS?
En la carpeta partials.

2 Estando en el archivo checkout.ejs, ¿cómo se hace para agregar el partial que representa al encabezado y está en el archivo head?
Arriba de todo el archivo, se inserta el código: <%- include('./partials/head')%>
*/



//* CLASE 22 - Crud: Episodio 1

//? Métodos HTTP

/* 
1 Para crear un nuevo registro en nuestra aplicación, ¿qué método es el más apropiado?
POST

2 ¿Cuál sería el mejor uso para el método PUT? 
Editar un registro.

3 ¿Cuál de las siguientes características corresponden al método GET?
Se guarda en caché.
Se accede por URL.

4 ¿Cuál sería el método más apropiado para eliminar información?
DELETE
*/

/* Creando nuestra primera ruta con Express 
const express = require ('express');
const router = express.Router()
router.get('/peliculas', function (req, res)  {
    res.send('Listado de películas')})
*/

//? Procesamiento GET

/* Usando query string para filtrar
const express = require('express');
const router = express.Router();
const controller = {
    productos: (req, res) => 
        res.send(req.query),    
    search: (req,res) => {
        let searchProduct = req.query.search;
        let usersResults= [];
        for(let i=0; i<users.product; i++) {
        if (product[i].name.includes(searchProduct)){
                userResults.push(product[i])
                }
        res.render('userResults', {userResults:userResults})
        }
    }
}
router.get('/productos', controller.productos)
router.get('/userResults', controller.search)
*/

/* Filtrando por precio
const express = require('express');
const router = express.Router();
const celulares = [
    {
        nombre: 'Motorola Moto E6 Plus',
        precio: 14999
    },
    {
        nombre: 'Motorola Moto G7',
        precio: 19999
    },
    {
        nombre: 'Alcatel 5033A',
        precio: 6999
    },
    {
        nombre: 'Samsung Galaxy A50',
        precio: 33499
    }
];
const controller = {
    celulares : (req, res) => 
    res.render('/celulares'),   
}
router.get ('/celulares', controller.celulares)
*/

//? Procesamiento POST

/* Preparando la constante para trabajar con POST
const express = require('express');
const app = express();
app.use(express.urlencoded({ extended: false }));
app.use(express.json());
*/

/* Recuperando información de POST
const express = require('express');
const router = express.Router()
router.post('/ver-body', (req,res) => {
    res.send(req.body)})
*/

/* Seteando un objeto con Data de POST
const express = require('express');
const router = express.Router();

let producto = {
    nombre: null,
    precio: null
};
router.get('/crear/producto', (req, res) => { res.render('crear')});
router.post('/crear/producto', (req, res) => {
    res.send(req.body)})
*/

//? Procesamiento PUT y DELETE

/* Asegurando la compatibilidad con PUT y DELETE 
const express = require('express');
const app = express();
const methodOverride = require('method-override')
app.use(methodOverride('_method'));
*/

/* Enviando datos de un formulario mediante PUT
<html>
  <head>
    <title>Formulario de registro</title>
  </head>
  <body>
    <form action="usuarios/actualizar?_method=PUT" method="POST">
    </form>
  </body>
</html>
 */

/* Vamos a tratar de crear una ruta JSON style
let peliculas = [
    {
        id: 1,
        titulo: 'Spider-Man: Lejos de casa',
        duracion: 129,
        genero: 'Aventura'
    },
    {
        id: 2,
        titulo: 'Toy Story 4',
        duracion: 100,
        genero: 'Animación'
    },
    {
        id: 3,
        titulo: 'X-Men: Fénix Oscura',
        duracion: 113,
        genero: 'Acción'
    }
];
const express = require('express');
const router = express.Router();
router.put('/pelicula/:id', (req, res) => {
    let idParams = req.params.id;
    peliculas.forEach(pelicula => {
       if (pelicula.id == idParams) {
           pelicula.titulo = req.body.titulo;
           pelicula.duracion = req.body.duracion;
           pelicula.genero = req.body.genero;
       }
    })
});
*/

/* Eliminando datos de un ARRAY 
let celulares = [
    {
        id: 1,
        nombre: 'Motorola Moto E6 Plus',
        precio: 14999
    },
    {
        id: 2,
        nombre: 'Motorola Moto G7',
        precio: 19999
    },
    {
        id: 3,
        nombre: 'Alcatel 5033A',
        precio: 6999
    },
    {
        id: 4,
        nombre: 'Samsung Galaxy A50',
        precio: 33499
    }
];
const express = require('express');
const router = express.Router();
router.delete("/celular/:id",(req,res)=>{
    let id = req.params.id
celulares = celulares.filter(celular => celular.id != id )
res.send(celulares)})
*/

//? Error 404

/* ¿Qué pasa si el usuario ingresa a una ruta que no existe?
const express = require('express');
const app = express();
const router = express.Router();
router.get('/', (req, res) => {
    res.send('Hola mundo');
});
app.use((req, res, next) => {
res.status(404).render('not-found')
})
app.use(router);
*/

//* CLASE 23 - CRUD: Episodio 2

//? Multer subiendo archivos

/* Preparando formularios para permitir la carga de archivos 
<html>
  <head>
    <title>Carga de imágenes</title>
  </head>
  <body>
    <form action="upload" method="POST" enctype="multipart/form-data">
    </form>
  </body>
</html>
*/

/* Usando Multer para la carga de archivos
const express = require('express');
const router = express.Router();
const multer = require('multer');
const path = require('path')
const storage = multer.diskStorage({
  destination: function (req, file, cb) {
    cb(null, '/tmp/my-uploads')
  },
  filename: function (req, file, cb) {
    const uniqueSuffix = Date.now() + '-' + Math.round(Math.random() * 1E9)
    cb(null, file.fieldname + '-' + uniqueSuffix)
  }
})
var upload = multer ({storage})
router.post('/register', upload.any(),usersController.save);
*/

//? Validación

/* ¡Ahora vamos a validar nuestra foto de perfil! 
var upload = multer({ storage: storage })
app.post('/register', upload.single('avatar'), (req, res, next) => {
const file= req.file
if (!file) {
    const error = new Error ('por favor seleccione un archivo')
error.httpStatusCode= 400
return next(error)
}
res.send(file)
})
*/

//? Hacia la clase en vivo

/*  
1 ¿Qué significan las siglas CRUD?
Create, Read, Update, Delete

2 ¿A través de qué método HTTP podemos enviar datos al servidor de forma segura?
POST

3 ¿Cuál es el método HTTP para modificar un recurso de forma total?
PUT

4 ¿Cómo utilizamos el middleware Method Override? Habiéndolo requerido de la siguiente forma:
const methodOverride = require('method-override');
app.use(methodOverride(_method))

5 ¿Qué métodos de fs se usan para escribir un archivo?
writeFile() writeFileSync() 

6 ¿Qué métodos usamos para subir archivos con Multer?
array(), single(), any()
*/

//* CLASE 25 - Middlewares

//? Middlewares: Aplicación Global

/* Agregando el middleware express.json()
const express = require('express');
const app = express();
const middlewareJSON =express.json()
app.use(middlewareJSON)
const router = express.Router();
router.post('/crear-usuario', (req, res) => {
    console.log(req.body);
    res.send('El usuario se creó con éxito');
});
app.use(router);
app.listen(3000);
*/

/* Sitio en mantenimiento
const express = require('express');
const app = express();
let enMantenimiento = false;
app.use(function (req, res, next){
    if (enMantenimiento === true) {
        res.render("en-mantenimiento")
    } else{
    next()
    }
})
*/

/* Agregando la propiedad usuario
const express = _require('express');
const app = express();
const usuario = {
    nombre: 'Máximo',
    apellido: 'Cozzetti'
};
app.use(function (req, res, next){
   usuario: req.usuario = usuario
    next();
})
*/

//? Middlewares: aplicación por ruta

/* Agregando middleware en la ruta "subir-archivo"
const express = require('express');
const router = express.Router();
const multer = require('multer');
const storage = multer.diskStorage({
  destination: function (req, file, cb) {
    cb(null, '/tmp/my-uploads')
  },
  filename: function (req, file, cb) {
    cb(null, file.fieldname + '-' + Date.now())
  }
}); 
const upload = multer({ storage: storage });
router.post('/subir-archivo', upload.any(), fileController.upload); //Agregar el middleware de multer
*/

/* Contando visitas
const express = require('express');
const router = express.Router();
const homeController = require('../controllers/homeController');
const estadisticasController = require('../controllers/estadisticasController');
function visitasMiddleware (req, res, next){
estadisticasController.contarVisita(req)
next()
}
router.get('/home', visitasMiddleware, homeController.index); //Agregá la función visitasMiddleware como segundo parámetro de tu ruta
*/

/* Redirigiendo a la HOME
const express = require('express');
const router = express.Router();
const OldController = require('../controllers/OldController');
function redirigir (req, res, next) {
     res.redirect('/')
}
router.get('/ruta-en-desuso', redirigir,OldController.index); //Agregá la función redirigir como segundo parámetro de tu ruta
*/

//? Introducción a express validator

/* Ejercitación 
const express = require('express');
const router = express.Router();
const UsuarioController = require('../controllers/UsuarioController');
const {check, validationResult,body} = require('express-validator')
router.post('/registro', [check('email').isEmail(), check('password').isLength({min : 6})], UsuarioController.registro);
*/

//? Express validator avanzado

/* Ejercitación 
const express = require('express');
const router = express.Router();
const { validationResult, body } = require('express-validator');
const userController = {
  login: (req, res) => {
    const errores = validationResult(req);
    if ( !errores.isEmpty()) {
     res.render('login', {errores: errores.array()})
    }
    if (req.body.name == 'admin' && req.body.pass == 123) {
        res.redirect('/dashboard');
    }
  }  
}
*/

//* CLASE 26 - Armado de login: sesion y cookies

//? Session

/* Configurando session
const express = require('express');
const app = express();
const session = require('express-session')
app.use(session({secret : 'frase secreta'}))
*/

/* Cambiando idioma
const express = require('express');
const app = express();
const session = require('express-session');
app.use(session({secret: "frase secreta"}));
const cambiarIdioma = (req, res) => {
    req.session.idioma = req.query.idioma;
    res.redirect('/');
}
*/

/* Validando usuarios
const express = require('express');
const app = express();
const session = require('express-session');
app.use(session({secret: "frase secreta"}));
const admin = (req, res) => {
    if (req.session.admin) {
    } else {
        res.redirect("login")
    }
}
*/

//? Cookies

/* Setear cookie
var express = require('express');
var cookieParser = require('cookie-parser');
var app = express();
app.use(cookieParser());
const index = (req, res) => {
    res.cookie('ultimoAcceso', new Date())
}
*/

/* Preferencias de usuario
var express = require('express');
var cookieParser = require('cookie-parser');
var app = express();
app.use(cookieParser());
const index = (req, res) => {
    let estilo;
    if(req.cookies.estilo!= undefined){
        estilo=req.cookies.estilo;
    }else{
        estilo='default';
    }
    res.render('/', {estilo: estilo});
}
*/

/* Recomendados
const listadoProductos = {
    vestidos: [
        'vestido broderie',
        'vestido towel',
        'vestido voile',
    ],
    remeras: [
        'remera alforzas',
        'remera bordada',
        'musculosa',
    ]
}
const recomendados = (req, res) => {
    const preferencias = req.cookies.preferencias
const productos = listadoProductos[preferencias]
res.render ("/recomendados", {productos: productos})    
}
*/


//? Hashing

/* Probando hash
const bcrypt = require ('bcrypt')
const password = '123456';
const hash = bcrypt.hashSync(password, 10)
console.log(hash)
*/

/* Validando información hasheada
const bcrypt = require('bcrypt');
const hash1 = bcrypt.hashSync('123456', 10);
const hash2 = bcrypt.hashSync('123456', 10)
if (hash1==hash2){
    console.log('los hash son iguales')
}
*/

/* Utilizando el método compareSync
const bcrypt = require('bcrypt');
const password = '123456';
const passwordEncriptada = bcrypt.hashSync(password, 10);
if(bcrypt.compareSync(password,passwordEncriptada)){console.log('El password es correcto');
}	
*/

//* CLASE 28 - Diseño y relaciones

//? Introducción a bases de datos

/* 
1 ¿Cuáles de los siguientes datos necesito para conectarme a una base de datos?
Nombre de la base de datos. Servidor donde está. Usuario y contraseña.

2 En una base de datos, el lenguaje de SQL permite...
Crear estructuras en la base de datos. Consultar información. Actualizar información.

3 ¿Qué es una clave primaria?
Una clave que permite identificar en forma unívoca un registro.

4 Una clave primaria puede ser formada por:
Un dato único. Un conjunto de datos
*/

//? Tablas

/* 
1 ¿Qué es un diagrama relacional?
La representación de las tablas en la base de datos.

2 ¿Cómo se lee?
Hay 3 tablas llamadas "Generos", "Artistas", "Bandas".

3 ¿Qué campos faltan?
nombre fantasía, edad, id (pk)
*/

//? Relaciones

/* 
1 ¿Qué tipos de relaciones existen en las bases de datos relacionales?
Uno a uno. Uno a muchos. Muchos a muchos.

2 ¿Qué cambios proponés?
Agregar la columna persona_id en la tabla Mascotas.

3 ¿Qué es una clave foránea?
Una referencia a la clave primaria de otra tabla.

4 ¿Qué cambios proponés?
Crear una tabla intermedia.

5 ¿Cómo se lee la siguiente relación?
Un jugador esta relacionado con un equipo. Un equipo esta relacionado con muchos jugadores.
*/

//? Tipos de datos

/*
1 ¿Qué tipos de datos podemos ver en SQL?
Texto, numerico, fecha

2 Dentro de los tipos de datos FECHA existen....
Date, datetime, time

3 Dentro de los tipos de datos TEXTO existen....
Varchar, char, text
*/

//? Constraints

/*
1 Cuando hablamos de un CONSTRAINT nos referimos a...
limitaciones en tipos de datos de una columna de la tabla.

2 Si quisieras establecer un campo que sí o sí se tenga que rellenar, ¿qué constraint deberías usar?
NOT NULL

3 Si quisieras que un dato no se repita jamás en una columna, ¿qué tipo de restricción usarías?
UNIQUE

4 ¿Para qué sirve la restricción PRIMARY KEY?
Para identificar de forma única cada fila de la tabla
*/

//? Create, drop y alter

/* Beneficios
1 Ingresá la consulta que creaste.
CREATE TABLE tipo_cliente (
id_tipo_cliente INT(6) NOT NULL,
PRIMARY KEY (id_tipo_cliente),
titulo VARCHAR(20) NOT NULL
)
*/

/* Fe de erratas (cosas que pasan)
1 Recordá escribir las sentencias SQL en mayúscula.
ALTER TABLE tipo_cliente
ADD porcentaje_descuento TYNYINT(3) UNSIGNED
*/

//? Foreign Keys

/* 
1 ¿Cómo y con qué se relaciona una Foreing Key?
Con una clave primaria de otra tabla.

2 ¿Cuántas foreing keys puede haber en una tabla?
Infinitas, siempre depende de las tablas que tengamos que relacionar y el espacio en memoria.
Una por cada tabla que relacionemos.
*/

//* CLASE 29 - Manipulación y consulta de datos

//? Insert, update y delete

/* Nuevos géneros de música
INSERT INTO musimundos.generos(id, nombre)
VALUES(26, 'Cumbia');
*/

//? Select

/* ¿Qué álbumes tenemos?
Big Ones
*/

/* Control de ventas 
+49 07112842222
*/

//? Where y Order by

/* 
1 Insertá el nombre del tercer cliente que obtuviste.
Michelle

2 Insertá el nombre de la quinta canción que obtuviste.
Inject The Venom

3 Seleccioná el nombre del primer cliente que te aparezca.
Enrique

4 Insertá el nombre del tercer género que hayas obtenido.
Blues

5 Seleccioná el nombre del séptimo cliente que encuentres.
Frank
*/

//? Beetween y like

/*  
1 Insertá el nombre de la cuarta canción que obtuviste.
Inject The Venom

2 Insertá el nombre del último género que obtuviste.
Electronica/Dance

3 Ingresá el nombre de la segunda canción que hayas obtenido.
C.O.D
*/

//? Limit y offset

/* 
1 Insertá el ID del álbum de las tres canciones que obtuviste, en orden, sin espacios y separados por coma.
227,229,253

2 Insertá el compositor de la quinta canción que obtuviste.
Santana
*/

//? Alias

/* 
Insertá el primer nombre de medio que obtuviste.
MPEG audio file
*/

//? Funciones de alteración

/*
1 Ingresá el primer resultado que obtuviste, sin comillas.
La cancion For Those About To Rock (We Salute You) fue compuesta por Angus Young, Malcom Young, Brian Johnson

2 Seleccioná el mes que dio la consulta.
12
*/

//* CLASE 30

//? Joins

/* 
1 Seleccioná la cuarta canción que te devuelva la consulta.
Restless and Wild

2 Ingresá el título del álbum en la posición número 10.
Stormbringer

3 Seleccioná el nombre de la cuarta canción que obtuviste de la consulta.
Inject The Venom
*/

//? Distincts

/* 
1 Ingresá el título que figura en la posición 4.
IT Manager
*/

//? Group by

/*
1 ¿Para qué nos sirve Group by?
Para agrupar registros similares.

2 Genera una consulta a la base Musimundos que cuente todas las canciones por genero y las agrupe por id_genero. Seleccioná el total del quinto registro.
12
*/

//? Funciones de agregación

/* 
1 Generá una consulta en la base de datos que traiga la cuenta de todos los clientes que son de Brazil.
5

2 Hacé una consulta a la base de datos que sume el total de todas las facturas que emitió la empresa.
2328.60

3 Hacé una consulta a la base de datos para saber cuál es el archivo con menor peso en bytes.
38747
*/

//? Having

/* 
1 Ingresá el país correspondiente al segundo registro de la respuesta a la consulta.
Canada

2 Ingresá la ciudad correspondiente al primer registro de la respuesta a tu consulta.
Berlin
*/

//? Hacia la clase en vivo

/* 
Canciones por género
81

Duración de los albums
306657.3750

Descuento
13.86
*/

//* CLASE 31 - Introducción, modelos y consultas básicas

//? Promesas

/* 
1 Las promesas son funciones que permiten:
Ejecutar código asincrónico de forma eficiente.

2 A veces necesitamos que dos o más promesas se resuelvan para realizar cierta acción. 
Promise.all()

3 En caso de NO obtener un resultado en la ejecución de algún código, se genera un error. 
.catch()

4 A veces los .then() suelen tener promesas dentro. 
Utilizar otro .then()

5 Es una función asincrónica, la cual devolverá un resultado, o no. Además permite que el código se siga ejecutando.
.then()
*/

/* Utilizando promesas
buscarProducto(1)
.then(function(producto){
    console.log(producto)
})
*/

/* ¿Y si la promesa falla?
buscarProducto(1).then(producto => {
    console.log(producto);
}).catch((error) => {
    console.log(error);
})
*/

//? Sequelize y configuración

/* 
1 ¿Para qué sirve un ORM?
Sirve para "transformar" las tablas de una base de datos, en una serie de entidades que simplifiquen las tareas básicas para manipular los datos.

2 Dentro del patrón de diseño MVC, ¿qué representa un modelo?
Contiene una representación de los datos que maneja el sistema, su lógica de negocio, y sus mecanismos de persistencia.

3 ¿Qué es Sequelize?
Es un ORM basado en promesas para Node.js que soporta bases de datos relacionales como MySQL.

4 El método define() nos permite definir asignaciones entre un modelo y una tabla. 
Un alias que identifica al modelo, un objeto con la configuración de las columnas en la base de datos y un objeto con configuraciones adicionales.

5 ¿Qué método debemos usar para buscar todos los datos registrados en una tabla?
findAll()
*/

//? Modelos

/* Creando un modelo
const Sequelize = require('sequelize');
const sequelize = require('../database');
const Usuario = sequelize.define(
  'usuarios', {
    nombre:  Sequelize.STRING,
    email:  Sequelize.STRING,
    password:  Sequelize.STRING,
  }
);
module.exports = Usuario;
*/

/* Evitando errores a la hora de crear un modelo
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const Usuario = sequelize.define('usuarios',{
    nombre: Sequelize.STRING,
    email: Sequelize.STRING,
    password: Sequelize.STRING,
},
{
  timestamps: false
}
);
module.exports = Usuario;
*/

//? findAll, findByPk, findOne

/* findAll
const db = require('../database/models');
let usuarios = []
db.Usuario.findAll()
.then((resultados) => {
    usuarios = resultados
})
*/

/* findByPk
const db = require('../database/models');
let controller = {
    profile: (req, res) => {
        db.Usuario.findByPk(req.params.id).then((resultado) => {
           console.log(resultado)
        })
    }
}
*/

/* findOne
const db = require('../database/models');
db.Usuario.findOne({
    where: {
        nombre: 'John'
    }
}).then((resultado) => {
    console.log(resultado)
});
*/

//? Where y operadores

/* Trayendo todas las películas
const Peliculas = require('model/peliculas.js');
Peliculas.findAll().then(resultados=> {
  console.log(resultados);
  })
*/

/* Trayendo pelis por ID
const Peliculas = require('model/peliculas.js');
Peliculas.findByPk(1)
.then(resultado=> {
  console.log(resultado);
  })
*/

//? Order y limit

/* Trayendo productos ordenados
const Producto = require('model/productos.js');
Producto.findAll({
  order: [['precio', 'ASC']]
}).then(productos => {
  console.log(productos)
});
*/

/* Paginando resultados
const Producto = require('model/productos.js');
Producto.findAll({
  limit: 5
}).then(productos => {
  console.log(productos)
});
*/

//? Hacia la clase en vivo

/* Desafío
'use strict';
module.exports = (sequelize, DataTypes) => {
    const product = sequelize.define('Product',  {
            id: DataTypes.INTEGER,
            nombre:  DataTypes.STRING(200),
            descripcion: DataTypes.TEXT,
            precio: DataTypes.DECIMAL
        }, {
            tableName: 'productos',
            timestamps: false
        });
  return product;
};
*/

/* Debemos completar el archivo productsController.js:
const db = require('../database/models') 
const controller = {
  index: (req, res) => {
     return res.send('Listado de productos');
  }
} 
module.exports = controller;
*/

/* hacer la consulta de TODOS los productos existentes en la base de datos.
const db = require('../database/models'); 
const controller = {
  index: (req, res) => {
    db.Product.findAll()
            .then(function (Product) {
                res.send(Product)
        })
  }
} 
module.exports = controller;
*/

/* Ahora nuestro cliente nos solicita buscar un producto a partir de su id
const db = require('../database/models');
const controller = {
  index: (req, res) => {
     db.Product
        .findAll()
        .then(products => {
           return res.send(products);
        })
        .catch(err => {
           return res.send(err)
        })
  },
  porId: (req, res) => {
     db.Product.findByPk(req.params.id)
     .then(product => {
           return res.send(product);
        })
        .catch(err => {
           return res.send(err)
        })
  }
}
*/

/* Para finalizar, nuestro cliente —bastante satisfecho— nos solicita un reporte sencillo. 
const db = require('../database/models');
const Op = db.Sequelize.Op;
const controller = {
   index: (req, res) => {
      db.Product
         .findAll()
         .then(productos => {
            res.send(productos);
         })
         .catch(err => {
            res.send(err)
         })
   },
   porId: (req, res) => {
      db.Product
         .findByPk(req.params.id)
         .then(producto => {
            res.send(producto);
         })
         .catch(err => {
            res.send(err)
         })
   },
   porPrecio: (req, res) => {
      db.Product
         .findAll({
            where: { precio: { [Op.gte]: 50000 } },
            order: [['nombre', 'ASC']],
            limit: 10
         })
         .then(producto => {
            res.send(producto);
         })
         .catch(err => {
            res.send(err)
         })
   },
}
module.exports = controller;
*/

//* CLASE 32 - Manipulación de datos

//? Create

/* Creando un usuario
const Usuario = require('model/usuario.js');
Usuario.create({
    nombre:"hola",
    email:"jose@gmail.com",
    password:"casacasa"
})
*/

/* Creando usuarios
const Pelicula = require('model/pelicula.js');
Pelicula.bulkCreate([
    {titulo:"pokemon",
    genero:"dibujo"},
{titulo:"dragon",
    genero:"dibujo"
    }
])
*/

/* Productos web
const Producto = require('model/producto.js');
const productoController = {
  create: (req, res) => {
    Producto.create({
   nombre: req.body.nombre,
   precio:req.body.precio
  } )
  }
}
*/

//? Update

/* Actualizando el precio
const Producto = require('model/producto.js');
Producto.update(
    { precio: 1234 },
    {  where: { id : 1 }  }
)
*/

/* Actualizando serie
const Serie = require('model/serie.js');
Serie.update(
    { genero:"sitcom" },
    {  where: { genero : "comedia" }  }
)
*/

/* Actualizando usuario
const Usuario = require('model/usuario.js');
Usuario.upsert(
    {email: "casa@dh.com", edad: 12 })
*/

//? Destroy/Soft deletes

/* Eliminar una película
const Pelicula = require('model/pelicula.js');
Pelicula.destroy({    
    where: { id : 3}
})
*/

/* Eliminar un usuario
const Usuario = require('model/usuario.js')
Usuario.destroy({
    where: { email : "kenny@south-park.com"}
})
*/

/* Eliminar varios usuarios 
const Sequelize = require('sequelize');
const Usuario = require('model/usuario.js');
const Op = Sequelize.Op;
Usuario.destroy({
    where: {
         email: { [Op.like]: '%aol.com'}
    }
})
*/

//? Hacia la clase en vivo

/* Desafío Sequelize
const db = require('../database/models');
const controller = {
  almacenarEnDB: (req, res) => {
    db.Product.create({
      id: req.params.id,
      nombre: req.body.nombreProducto,
      descripcion: req.body.descripcionProducto,
      precio: req.body.precioProducto
    })
    res.redirect('/productos')
  }
}
module.exports = controller;
*/

/* Para usar el método del controlador que completamos anteriormente, se hace necesario ahora disponer de una ruta que lo implemente. La ruta será /productos.
const express = require('express');
const router = express.Router(); 
const productsController = require('../controllers/productsController'); 
router.get('/', productsController.index);
router.post('/', productsController.almacenarEnDB);
module.exports = router;
*/

/* Ahora nos interesa completar el método editarRegistro presente en el controlador.
const db = require('../database/models');
const controller = {
   almacenarEnDB: (req, res) => {
      db.Product
         .create({
            nombre: req.body.nombreProducto,
            precio: req.body.precioProducto,
            descripcion: req.body.descripcionProducto
         })
         .then(producto => {
            res.redirect('/productos');
         })
   },
   editarRegistro: (req, res) => {
      db.Product.update(
         {
            id: req.params.id,
            nombre: req.body.nombreEditado,
            descripcion: req.body.descripcionEditada,
            precio: req.body.precioEditado
         },
         {
            where: { id: 3 }
         })

      res.redirect('/productos')
   },
}
module.exports = controller;
*/

/* Ya falta poco para completar el proceso de CRUD. Ahora nuestra misión será la de completar el método borrarRegistro presente en el controlador.
const db = require('../database/models');
const controller = {
   almacenarEnDB: (req, res) => {
      db.Product
         .create({
            nombre: req.body.nombreProducto,
            precio: req.body.precioProducto,
            descripcion: req.body.descripcionProducto
         })
         .then(producto => {
            res.redirect('/productos');
         })
   },
   editarRegistro: (req, res) => {
      db.Product
         .update(
            {
               nombre: req.body.nombreEditado,
               precio: req.body.precioEditado,
               descripcion: req.body.descripcionEditada
            },
            {
               where: { id: req.params.id }
            }
         )
         .then(() => {
            res.redirect('/productos');
         })
   },
   borrarRegistro: (req, res) => {
      db.Product.destroy({
         where: { id: req.params.id }
      })
      res.redirect('/productos')
   },
}
module.exports = controller;
*/

/* Finalmente, necesitamos llevar a cabo el proceso de edición y el proceso de eliminar.
const express = require('express');
const router = express.Router(); 
const productsController = require('../controllers/productsController'); 
router.get('/', productsController.index);
router.post('/', productsController.almacenarEnDB);
router.put('/:id', productsController.editarRegistro);
router.delete('/:id', productsController.borrarRegistro);
module.exports = router;
*/

//* CLASE 33 - Relaciones y CRUD completo

//? Relaciones 1:N

/* Género
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const Genero = require('model/genero.js');
const Pelicula = sequelize.define('peliculas',{
    titulo: Sequelize.STRING,
    genero_id: Sequelize.INTEGER,
});
Pelicula.belongsTo(Genero, {
    as: "genero",
    foreignKey: 'genero_id'
})
module.exports = Pelicula;
*/

/* Para este ejercicio nuestra meta va a ser, luego de la definición del modelo de Genero, vincular a este con el modelo Pelicula.
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const Pelicula = require('model/pelicula.js');
const Genero = sequelize.define('generos',{
    nombre: Sequelize.STRING,
});
Genero.hasMany(Pelicula, {
    foreignKey: 'genero_id',
    as: 'genero'
})
module.exports = Genero;
*/

/* En este ejemplo, tenemos el modelo Pelicula que tiene creada una relación con el modelo Genero.
const Pelicula = require('model/pelicula.js');
Pelicula.findByPk(1,{ include: ['genero'] })
.then(pelicula => console.log(pelicula.genero.nombre))
*/

/* crear un producto cuyo nombre sea "Falcon 9" y crear en el mismo método un usuario asociado a ese producto que tenga como nombre "Elon" y como apellido "Musk".
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const Usuario = sequelize.define('usuarios',{
    nombre: Sequelize.STRING,
    apellido: Sequelize.STRING,
});
const Producto = sequelize.define('productos',{
    nombre: Sequelize.STRING,
    usuario_id: Sequelize.INTEGER,
});
const Creador = Producto.belongsTo(Usuario, { as: 'creador' });
Producto.create({nombre: 'Falcon 9', creador: {nombre: 'Elon',apellido: 'Musk'}},{include: [Creador]})
*/

//? Relaciones N:M

/* Películas de actor
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const PeliculaActor = sequelize.define('pelicula_actor',{
    pelicula_id: {
      type: Sequelize.INTEGER,
      references: {
        model: 'Pelicula',
        key: 'id'
      }
    },
    actor_id: {
      type: Sequelize.INTEGER,
      references: {
        model: 'Actor',
        key: 'id'
      }
    }
});
module.exports = PeliculaActor;
*/

/* Relaciones Pivot
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const Actor = require('model/actor.js');
const Pelicula = require('model/pelicula.js');

const PeliculaActor = sequelize.define('pelicula_actor',{
    pelicula_id: {
      type: Sequelize.INTEGER,
      references: {
        model: 'Pelicula',
        key: 'id'
      }
    },
    actor_id: {
      type: Sequelize.INTEGER,
      references: {
        model: 'Actor',
        key: 'id'
      }
    }
});
PeliculaActor.belongsTo(Pelicula,{foreignKey:"pelicula_id"})
PeliculaActor.belongsTo(Actor,{foreignKey:'actor_id'})
module.exports = PeliculaActor;
*/

/* Películas actor, toma 3
const Sequelize = require('sequelize');
const sequelize = require('../database'); 
const Actor = require('model/actor.js');

const Pelicula = sequelize.define('peliculas',{
  titulo: Sequelize.STRING,
  genero_id: Sequelize.INTEGER,
});

 Pelicula.belongsToMany(Actor, {
   foreignKey: "pelicula_id",
    as: "actores", 
    through: 'PeliculaActor' })

module.exports = Pelicula;
*/

/* Buscando actores
const Pelicula = require('model/pelicula.js');
 Pelicula.findByPk(1, {include: ['actores']})
 .then(pelicula => console.log(pelicula.actores))
*/

/* Agregando actores
const Pelicula = require('model/pelicula.js');
Pelicula.findByPk(1).then(pelicula => {
  pelicula.setActores([3, 5, 8])
});
*/

//? Hacia la clase en vivo

/* Desafio
'use strict'; 
module.exports = (sequelize, DataTypes) => {
const product = sequelize.define('Product', {
     nombre: DataTypes.STRING(200),
     descripcion: DataTypes.TEXT,
     precio: DataTypes.DECIMAL,
  }, {
          timestamps: false,
          tableName: 'productos',
  }); 
  product.associate = models => {
    product.belongsTo(models.Brand,{
        as: 'brand',
        foreignKey: 'marca_id'
    })
} 
  return product;
};
*/

/* Ahora, nuestra misión será crear una relación opuesta, la de N a 1. Pues, una marca tiene muchos productos.
'use strict'; 
module.exports = (sequelize, DataTypes) => {
    const brand = sequelize.define('Brand', {
      nombre: DataTypes.STRING(),
    }, {
          timestamps: false,
          tableName: 'marcas',
  }); 
    brand.associate = models => {
      brand.hasMany(models.Product,{
      as: 'products',
      foreignKey:"brand_id"
     })
    } 
    return brand;
};
*/

/* crear una relación adicional que permita consultar los colores que tiene asignado un producto
'use strict'; 
module.exports = (sequelize, DataTypes) => {
const product = sequelize.define('Product', {
     nombre: DataTypes.STRING(200),
     descripcion: DataTypes.TEXT,
     precio: DataTypes.DECIMAL,
  }, {
          timestamps: false,
          tableName: 'productos',
  }); 
product.associate = models => {
  product.belongsTo(models.Brand, {
    as: 'brand',
    foreignKey: 'marca_id'
  }); 
  product.belongsToMany(models.Color,{
    as: 'colors',
    through: 'colores_productos',
  })
} 
  return product;
};
*/

/* Con todo lo anterior, solamente nos queda generar la consulta dentro del controlador para poder ver la marca de un producto y sus colores.
const db = require('../database/models'); 
const controller = {
  index: (req, res) => {
     db.Product
        .findAll({	
          include:['brand', 'colors']
   })
        .then(productos => {
           res.send(productos);
        })
        .catch(err => {
           res.send(err)
        })
  }
} 
module.exports = controller;
*/

//* CLASE 35 - APIs

//? REST

/* 
1 ¿Qué es REST?
Representational

2 ¿Qué es REST?
Un tipo de arquitectura

3 ¿Qué es un endpoint?
Un archivo de nuestro proyecto, un recurso del servidor
*/

//? Creación de una API propia

/* 
1 ¿Qué parte de la siguiente URL hace referencia a la colección?
/actores/1/nombre
"/actores"

2 ¿Cuál es el primer paso para crear una API?
Identificar el Objeto Modelo.

3 Según las buenas prácticas, ¿cómo solemos nombrar a nuestros recursos?
Sustantivos comunes.
*/

//? Hacia la clase en vivo

/* 
1 ¿Qué significa el cacheo de datos en REST?
Una memoria intermedia que almacena datos

2 ¿En qué formato devuelve los datos el servidor después de haber hecho una solicitud?
JSON, RAW, XML, URL-encoded

3 ¿Cuál de las siguientes opciones no es un método válido por el cual podemos manipular los datos de nuestra API?
Destroy

4 Una vez identificado el Objeto Modelo, ¿cuál es el siguiente paso para la exitosa creación de una API?
Crear nuestras rutas.
*/

//* CLASE 36 - Consumo de APIs propias y de terceros

//? Postman

/* 
1 Postman es...
-Un cliente HTTP para probar servicios web.
-Una herramienta que permite testear, consumir y depurar API REST, monitorizarlas, escribir pruebas automatizadas, documentarlas, mockearlas y simularlas.

2 Diferencias entre el servidor REST y el cliente REST.
-Un ejemplo: Twitter tiene datos que quiere compartir (Tweets), por lo que expone una API por un servidor REST. Si deseamos escribir una aplicación que use esa API para buscar y exponer tweets de un usuario, nuestra aplicación sería el cliente REST.
-El servidor responde a las solicitudes. El cliente realiza solicitudes.

3 Postman permite enviar peticiones con los métodos..
GET, POST, PATCH, DELETE, PUT
*/

//? Hacia la clase en vivo

/* 
1 ¿Cuál es la finalidad de Node Fetch?
Hacer solicitudes HTTP a una API

2 ¿Cuántos métodos then() debe llevar una petición de tipo FETCH?
Debe llevar dos métodos then()

3 Si hacemos un pedido por POST con Postman, ¿en qué parte debemos enviar la información?
En la pestaña de body.
*/

//* CLASE 37 - Manipulando elementos con Javascript

//? Vinculación

/* 
1 Existen dos formas de vincular JavaScript con nuestro documento HTML. La más recomendada es:
La vinculación externa

2 Podemos tener un solo archivo de JavaScript vinculado a nuestro documento HTML.
Falso

3 Solo en una de las opciones se ejecutará el console.log(). Seleccioná cuál.
<script> console.log('Vinculando JS') </script>
*/

/* A vincular
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>JS Front</title>
  </head>
  <body>
    <p>Podés abrir la consola del navegador para chequear los resultados</p>
    <script src="script.js"></script>
  </body>
</html>
*/

//? Objeto window y document

/* 
1 JavaScript nos permite interactuar con el front-end del usuario siempre y cuando se haga una petición al servidor.
Falso

2  ¿Qué es el DOM?
La representación en objetos que hace JavaScript del documento HTML.

3 El objeto window representa la ventana donde estamos navegando.
Verdadero

4 Mediante el objeto document podemos...
Leer todos los elementos del HTML y modificarlos, si así lo quisiéramos.
*/

//? DOM selectores

/* Manipulando elementos con JavaScript
window.addEventListener('load', function() {
  let tituloPelicula=document.querySelector('h2')
});
*/

/* Manipulando elementos con JavaScript II
window.addEventListener('load', function() {
  let parrafos = document.querySelectorAll('p')
});
*/

/* Manipulando elementos por id
window.addEventListener('load', function() {
let pulpFiction = document.getElementById('pulp-fiction')
});
*/

/* Manipulando elementos por nombre de clase 
window.addEventListener('load', function() {
let  barraDeNavegacion = document.getElementByClassName("nav-bar")
});
*/

//? Modificando el DOM

/* Sumando texto a un elemento con contenido 
window.addEventListener('load', function() {
document.querySelector('h3').innerText += ' usando código';
});
*/

/* Agregando etiquetas
window.addEventListener('load', function() {
document.querySelector('body').innerHTML += '<mark>Javascript ROCKS</mark>';
});
*/

//? Modificando estilos

/* Modificando estilos
window.addEventListener('load', function () {
  document.querySelector('body').style.backgroundColor = "lightskyblue";
  document.querySelector('h2').style.textAlign = 'center';
  document.querySelector('h4').style.fontStyle = 'italic'
});
*/

/* ¡Modificando estilos a varios elementos a la vez!
window.addEventListener('load', function () {
  let libros = document.querySelectorAll('li')
  for (let libro of libros) {
    libro.style.color = 'orange'
  }
});
*/


//? Modificando clases

/* Agregando clases a un elemento
window.addEventListener('load', function() {
let cita = document.querySelector('div');
cita.classList.add("container")
});
*/

/* Sacando clases a un elemento
window.addEventListener('load', function() {
let cita = document.querySelector('h1');
cita.classList.remove("titulo")
});
*/

/* Alternando clases
window.addEventListener('load', function() {
let h1 = document.querySelector('h1');
cita.classList.toggle('titulo-tuneado');
});
*/

//? Hacia la clase en vivo

/* Desafío: ¡ups cometimos un error!
window.addEventListener('load', function(){
let horrorOrtografico=document.querySelector('.title')
horrorOrtografico.innerHTML = 'Bienvenidos a mi <em>sitio web</em>';
})
*/

/* Desafío: Capturando elementos del documento
window.addEventListener('load', function(){
let theSubtitle = document.querySelector('.subtitle');
let paragraphs = document.querySelectorAll('p');
let navAnchors = document.querySelectorAll("#main-navbar a");
let mainImage = document.querySelector('#main-image');
})
*/

/* Desafío: ¡Cuidado con la clase!
const listItems = document.querySelectorAll("#cont01 li");
for (let i = 0; i < listItems.length; i++) {
   if (listItems[i].classList.contains("alert-danger")) {
      listItems[i].classList.remove("alert-danger");
      listItems[i].classList.add("alert-success");
   }
}
*/

//* CLASE 38 - Agregando interacción con eventos

//? ¿Qué son los eventos?

/* 
1 Elegí cuál es la opción correcta para reemplazar los “?????” en la siguiente línea de código, en caso que queramos disparar un evento al hacer clic sobre el elemento:
  elemento.addEventListener(‘?????’, function(event){
})
"click"

2 ¿Cuál es el propósito de .preventDefault()?
Evitar que el elemento ejecute el evento que trae por default para que podamos manipularlo antes.
*/

/* Método load
window.addEventListener('load', function(){   
})
*/

/* Evento click
window.addEventListener('load', function() {
  let linkContacto = document.querySelector('.contacto');
   linkContacto.addEventListener('click',function(e){
     console.log("Hiciste click" )
   }) 
});
*/

/* Prevent default
window.addEventListener('load', function() {
 let formulario = document.querySelector('form')
formulario.addEventListener('submit', function(evento){
evento.preventDefault()
})
});
*/

//? Eventos de mouse

/* Mouseover
window.addEventListener('load', function () {
  let titulo = document.querySelector('h1')
  titulo.addEventListener('mouseover', function () {
    titulo.classList.add('titulo')
  })
});
*/

/* Mouseout
window.addEventListener('load', function () {
  let links = document.querySelectorAll('a')
  for (let link of links) {
    link.addEventListener('mouseout', function () {
      this.classList.toggle('dark-mode')
    })
  }
});
*/

//? Eventos de teclado

/* 
1 ¿Cuál de todas las propiedades de un evento de teclado es la que almacena el valor de la tecla presionada?
key

2 Cuál de las siguientes opciones es la correcta para reemplazar los “?????” en la siguiente línea de código, teniendo en cuenta que queremos enviar un alert cuando se libere la tecla después de haber sido presionada:
  elemento.????? = function(){
    alert(“¡se liberó la tecla!”)
}
onkeyup
*/

/* onkeydown
window.addEventListener('load', function() {
    let userName = document.querySelector('#userName')
 userName.addEventListener('keydown', function(event){
        if(event.key == "#" ) {
            alert("Está prohibido el uso de #hashtags!")
        }
    })
});
*/

/* onkeypress
window.addEventListener('load', function(){
let direccion = document.querySelector('#address')
 direccion.addEventListener('keypress', function(event){
         alert("Se presionó la tecla: "+ event.key );
    })
})
*/

//? Hacia la clase en vivo

/* No nos gusta la letra "x"
window.addEventListener("keypress", function(e) {
  let key =  e.key;
  const body = document.querySelector("body"); 
  if (key === 'x') {
     document.body.style.backgroundColor = "orange";
     //body.style.backgroundColor = "orange";
  }
})
*/

/* ¡Evitemos que esto se desenlace! 
window.addEventListener('load', function(){
    const specialAnchor = document.querySelector("a");
    specialAnchor.addEventListener("click", (event) => {
        event.preventDefault();
        this.style.color = "red"
        this.innerText = "este enlace no te llevará a ningún lado"
    })
})
*/

//* CLASE 39 - Interactuando con formularios

//? Eventos de formularios

/* 
1 El evento blur sirve para...
detectar que el usuario quitó el cursor de un input del formulario.

2 El evento focus sirve para...
detectar que el usuario situó el cursor en un input del formulario.

3 El evento change sirve para...
detectar cambios en el valor de un input.
*/

/* onfocus 
window.addEventListener('load', function(){
let elNombre = document.querySelector('#nombre')
elNombre.addEventListener('focus', function (){
    elNombre.style.backgroundColor  = "pink"
})
})
*/

/* onblur
window.addEventListener('load', function(){
    let elUsuario = document.querySelector('#user')
    elUsuario.addEventListener('blur',function(){
       elUsuario.style.backgroundColor = 'plum'
    })
})
*/

/* onchange 
window.addEventListener('load', function () {
   let miInput = document.querySelector('#miInput')
   miInput.addEventListener('change', function () {
      let body = document.querySelector('body')
      document.body.style.backgroundColor = 'red'
   })
})
*/

/* onsubmit
window.addEventListener('load', function(){
    let mensajeOculto = document.querySelector('h1')
    let miForm = document.querySelector('#miForm')
    miForm.addEventListener('submit', function(){
        miForm.style.display = "none"
        mensajeOculto.style.display = "block"
    })
})
*/

//? Validaciones

/* Prevent default
window.addEventListener('load', function() {
let formulario = document.querySelector('form')
formulario.addEventListener('submit', function (evento){
  evento.preventDefault()
})
});
*/

/* Validando campos
window.addEventListener('load', function() {
  let formulario = document.querySelector('form');
  formulario.addEventListener('submit', function(evento) {
    evento.preventDefault();
let nombre = document.querySelector('#nombre')
let password = document.querySelector('#password')
if (nombre.value == "" ){
  Console.log("Hubo un error en el nombre'")
}
if (password.value.length <= 4 ){
  Console.log("Hubo un error en el password")
}
  })
});
*/

//* CLASE 40 - Pedidos asincrónicos con Javascript

//? Fetch

/* Vamos a usar FETCH por GET
fetch('https://api.chucknorris.io/jokes/random')
.then(function(response){
    return response.json()
})
.then(function(data){
    console.log(data)
})
*/

/* 
1 Vamos a usar FETCH por POST
La URL y configuraciones de la conexión.

2 ¿Cuál de los siguientes es un elemento que puede aparecer dentro de la configuración del fetch?
method, headers, body, content-type
*/

//? Object location

/*  
1 Si utilizáramos el atributo href de location sobre la URL: https://www.youtube.com/results?search_query=peaky+blinders, ¿qué obtendríamos??
https://www.youtube.com/results?search_query=peaky+blinders

2 ¿Qué método del objeto location permite recargar el sitio??
location.reload()

3 Si utilizáramos el atributo location.search de la URL: https://www.youtube.com/results?search_query=peaky+blinders, ¿qué obtendríamos?
search_query=peaky+blinders

4 Si estamos en la URL: https://www.youtube.com/results?search_query=peaky+blinders, y teniendo en cuenta el código: "let query = new URLSearchParams(location.search)", ¿qué devolvería si implementáramos el método query.get(search_query)?
peaky+blinders
*/

//? Session storage y local storage

/* 
1 ¿Cuál es la diferencia entre sessionStorage y localStorage?
localStorage permite almacenar información por tiempo indeterminado y sessionStorage, no.

2 El método .setitem() de localStorage, ¿qué nos permite realizar?
Agregar valores asociados a una key en localStorage.

3 El método .removeitem() de sessionStorage, ¿qué nos permite realizar?
Remover valores asociados a una key en el sessionStorage.

4 El método .clear() de localStorage, ¿qué nos permite realizar?
Borrar todo el contenido de localStorage.

5 ¿Cuál de las siguientes es una de las características de sessionStorage?
Los datos se borran al cerrar la ventana del navegador.
*/

/* Local storage 
window.addEventListener('load', function(){ 
    let id = localStorage.getItem("id")
    let idValue = document.querySelector('#idValue')
  idValue.innerHTML = id 
})
*/

/* Session storage
window.addEventListener('load', function(){
localStorage.setItem('bgColor', "red")
localStorage.removeItem('font')
})
*/

//? Hacia la clase en vivo

/* ¡Saludando a nuestros visitantes! 
window.addEventListener('load', function(){
const h2 = document.querySelector("h2");
if(localStorage.getItem("user")) {
  h2.innerText = "Hola " + localStorage.getItem("user")
} else {
  h2.innerText = "Hola visitante"
}
})
*/

/* Recordando a la persona que nos visita
window.addEventListener('load', function(){
const button = document.querySelector("button");
const h2 = document.querySelector("h2");
button.addEventListener("click", function () {
  if(!localStorage.getItem("user")) {
     localStorage.setItem("user", JSON.stringify(userInfo))
  }
})
});
*/


//* CLASE 43 - Creando una aplicación con React

//? Introducción a React

/* 
1 ¿Qué es React?
Es una librería escrita en JavaScript para facilitar la creación de componentes interactivos.

2 ¿Qué sucede cuando alguna parte del DOM de mi sitio cambia?
React hace una comparación entre el Virtual DOM y el DOM real, para saber qué partes de mi sitio actualizar, ahorrando la necesidad de actualizar todo el sitio.
React realiza el proceso de Diffing que consiste en comparar las dos versiones (Virtual DOM y DOM real) para luego realizar el Reconciliation, que es la actualización de las partes de la vista que cambiaron.

3 React...
es capaz de identificar cambios en el DOM.
es una librería realizada por Facebook.
puede ser representado del lado del cliente y también del lado del servidor.

4 Si quisiera mejorar el rendimiento del front-end de mi sitio...
podría utilizar react

5 ¿Qué es el Diffing?
Es un proceso que hace React en el cual genera un DOM Virtual idéntico al DOM real y los compara constantemente, para así ir solo actualizando los fragmentos del DOM real que difieren en la comparación.
*/

//? Instalación y puesta en marcha

/*  
1 ¿Qué comandos podemos ejecutar para crear nuestro proyecto en React?
npm init react-app mi-app-de-react
npx create-react-app mi-app-de-react

2 ¿Cómo debo nombrar a mi proyecto en React?
mi-proyecto

3 En qué carpeta se encuentra el archivo principal “index.html”, que se va a cargar cuando el usuario ingresa a la URL de nuestra aplicación:
/public

4 ¿En qué carpeta se encuentran todos los archivos con los que vamos a trabajar nuestro proyecto en React?
/src

5 Una vez que nos encontramos en la raíz de nuestro proyecto, ¿qué comando debemos ejecutar para iniciarlo?
npm start
*/


//? Ecosistema de React

/* 
1 ¿Qué es Webpack?
Es un empaquetador de módulos donde su objetivo principal es crear un único archivo de JavaScript.

2 ¿Qué es Babel?
Es un traductor de código estable e interpretable que usa React.
Es una librería que cumple con la función de la transpilación, el cual es un proceso de traducción.

3 Webpack comúnmente se conoce como...
Module Bundler o Empaquetador de módulos.

4 Webpack y Babel...
presentan los archivos de configuración ocultos luego de ejecutar npm init react-app.
son librerías.
*/


//? Introducción a componentes

/* 
1 Al crear un componente stateless, ¿cuál debería ser una de las primeras líneas de nuestro archivo?
import React from 'react'

2 Si nos corresponde crear un componente llamado “Category”, ¿cuál debería ser la última línea de nuestro archivo?
export default Category;

3 Si te piden hacer un componente sin estado cuyo nombre sea “Saludar”, ¿cuál de las siguientes porciones de código es la correcta?
D
*/


//? JSX

/* 
1 ¿Cuál de las siguientes opciones es una de las consideraciones que debemos tener presente al momento de escribir código JSX?
Todas las etiquetas necesitan ser correctamente cerradas.

2 Si queremos iterar sobre un array en JSX, debemos utilizar los métodos:
.map() .filter() o .reduce()

3 Supongamos que estamos trabajando con JSX y deseamos disponer una imagen en alguno de nuestros componentes. ¿Cuál de las siguientes líneas de código es la correcta?
<img src= “/img/logoDH.jpg” alt=”Logo de Digital House”/>

4 Supongamos que deseamos imprimir el valor de alguna variable o deseamos generar alguna lógica dentro de nuestro componente. ¿Cuál de las siguientes líneas de código es la correcta?
<ul> { productos.map( producto => <li> producto </li> ) } </ul>
*/

//* CLASE 44 - Trabajando con componentes

//? Props

/* 
1 ¿Qué son las props?
Es información que le envía un componente padre a un hijo.

2 Tengo que enviar mucha información a un componente, por lo que pienso hacerlo en varias props. ¿Es correcto lo que pienso?
No, la información se envía una sola vez a un componente a través de props.

3 ¿Cuándo se define la información que va a ser enviada por prop?
Cuando se crea el componente.

4 Props es...
un objeto literal

5 ¿Cuál de las siguientes sentencias es incorrecta?
<Libro props={ {titulo:"Harry Potter"} }/>

6 Supongamos que tenemos un componente que se llama Saludo y queremos pasarle dos props. Las props que queremos pasarle serían las siguientes: 
titulo = “Hola mundo”
subtitulo = “¡Nunca paremos de aprender!”
<Saludo titulo="Hola mundo" subtitulo="¡Nunca paremos de aprender!"/>
*/

//? Prop types y default props

/* 
1 ¿Es verdad que las prop types pueden setear valores por defecto en caso de que un componente no tenga valor?
No, es mentira.

2 ¿Qué tipo de dato aceptan las prop types y las default props?
Un objeto literal.

3 ¿Cuál de las siguientes líneas de código es la correcta?
C
*/

//? Children

/* 
1 Si tuvieras que explicar la funcionalidad de los children, dirías que:
Los children permiten enviar y renderizar un componente o HTML dentro de otro.

2 Cuando definimos que un componente va a recibir elementos o componentes por children, estos se pueden imprimir en cualquier lugar del componente padre
No, es falsa

3 ¿Cómo hacemos para declarar que un componente puede recibir elementos por children?
A
*/

//? Styling

/* 
1 Al crear un componente,  ¿cómo podemos vincular un archivo CSS?
import “hojaDeEstiloComponente.css”;

2 Si queremos asignarle una clase a algún elemento de nuestro componente, ¿cómo deberíamos hacerlo?
<h1 className = ”titulo”>Bienvenido al sitio web</h1>

3 Aunque estemos modularizando nuestros estilos, para evitar conflictos al momento de renderizar el sitio, ¿cuál sería una buena práctica para evitar que se pisen nuestras clases entre sí?
No repetir nombre de clases entre hojas de estilos.
*/

//? Hacia la clase en vivo

/* 
1 ¿Qué son las props de un componente?
Son entradas de un componente de React. Son información que es pasada desde un componente padre a un componente hijo.

2 ¿Cómo definimos una props dentro del componente?
Escribiendo una función de JavaScript y, a la misma, le asignamos como parámetro props.

3 ¿Qué son los children de un componente?
Una propiedad con la que podremos traer a todos los hijos que definamos dentro del componente padre. 

4 ¿Cómo manejar los children dentro del componente?
props.children está disponible en cada componente. Contiene el contenido ubicado entre las etiquetas de apertura y cierre de un componente.

5 ¿Qué son las proptypes de un componente?
Son propiedades que permiten la verificación de tipos en las props de un componente.

6 ¿Para qué sirven las defaulProps de un componente?
Para establecer las props predeterminadas que recibirá un componente.
*/

//* CLASE 45 - El ciclo de vida de los componentes

//? Ciclos de vida

/* 
1 ¿Cuándo se ejecuta el método componentDidMount()?
Después de renderizarlo por primera vez.

2 ¿Cuándo se ejecuta el método componentDidUpdate()?
Cuando el componente sufra algún cambio de estado.

3 Tenemos el siguiente componente, en el cual tenemos un temporizador cada vez que se renderiza el componente. ¿Cuál sería el método correcto para eliminar el temporizador?
B

*/

//? Integración con APIs

/*  
1 ¿En qué fase del ciclo de vida de un componente solemos hacer el fetch al endpoint de una API? 
ComponentDidMount()

2 ¿Cuál línea de código es la correcta? 
A y C

3 Tenemos el siguiente componente definido:
.then(data=>{this.setState({gif:data.data.image_url})
*/


//* CLASE 46 - Enlazando los componentes de la aplicación

//? Instalando React Router Dom

/*
1 ¿Qué comando debemos ejecutar para instalar React Router DOM?
npm install react-router-dom

2 ¿Para qué sirve React Router DOM?
React Router es una librería para gestionar rutas en aplicaciones que utilicen React.
*/

//? Qué componentes nos provee React Router Dom

/* 
1 ¿Cuál de los siguientes son componentes que nos brinda React Router DOM?
BrowserRouter, Link, Route, Switch.

2 ¿Para qué usamos BrowserRouter?
Es como una envoltura de enrutación para nuestro proyecto.

3 ¿Para qué usamos el componente Link?
Permite indicar una ruta a la cual queremos navegar.

4 ¿Para qué usamos el componente Route?
Permite indicar qué componente se renderizará dependiendo de la ruta.

5 ¿Para qué usamos el componente Switch?
Permite renderizar al primer hijo Route que coincide con la ubicación.
*/

//? Creando la primera ruta y renderizando el componente específico

/*  
1 Seleccioná la opción correcta:
Route nos permite definir cuál componente se va a renderizar según la ruta especificada y para poder implementarlo debemos importarlo previamente.

2 Si quisiéramos que se renderice el componente de nombre “Login”, dentro de las props "component", ¿qué deberíamos colocar?
component={Login}

3 ¿Qué debemos colocar en Route para que renderice exactamente una ruta en particular y deje de ser genérica?
exact

4 Link crea un hipervínculo que nos permite navegar por nuestra aplicación. Si queremos navegar a  “/about”, ¿cómo deberíamos configurar Link?
<Link to="/about">About</Link>
*/

//? Cómo hacer switch de rutas y componentes

/* 
1 Seleccioná la opción correcta:
Switch nos permite que solo se renderice el primer hijo Route que coincida con la locación o URL actual.

2 Seleccioná la opción correcta:
En caso que no usemos Switch todas las rutas que cumplan con la condición se renderizan.
*/

//? Cómo trabajar con rutas parametrizadas

/* 
1 Seleccioná la opción correcta:
match es un objeto literal que tiene, a su vez, varias propiedades.

2 Seleccioná la opción correcta:
La propiedad params dentro de match contendrá todos y cada uno de los parámetros enviados en la ruta.
*/

//? Hacia la clase en vivo

/*  
1 Para permitir que nuestra aplicación de React se comporte como una SPA real, tendremos que instalar una librería adicional que nos permita gestionar el sistema de ruteo de una manera óptima e inteligente. ¿Cuál debería ser el paquete que debemos instalar?
npm install react-router-dom

2 ¿Que debemos hacer para lograr implementar los componentes que trae el módulo de react-router-dom?
import {BrowserRouter, Link, Route, Switch} from 'react-router-dom';

3 ¿Cuál de los siguientes componentes es el enrutador general y necesario para administrar las rutas de nuestro proyecto?
<BrowserRouter>

4 ¿Cuál de las siguientes líneas de códigos es la correcta para configurar qué componente se debe renderizar en base a la ruta que se esté accediendo?
<Route path="/contact" exact={true} component={Contact}/>

5 ¿Cuál es el componente que permite albergar todos los componentes <Route/>  que tengamos definidos y además nos ofrece una forma muy sencilla de controlar cuando se pretende acceder a una ruta desconocida?
<Switch>

6 Cuando queremos comenzar a trabajar con rutas parametrizadas, lo primero que tenemos que hacer es definirlas. En base a esto, ¿cuál de las siguientes rutas parametrizadas está correctamente definida?
<Route path="/product/:id" component={Product />

7 ¿Cómo podemos hacer si queremos almacenar o acceder al valor que viajó por una ruta parametrizada?
const id = props.match.params.id;
*/



//* CLASE 47 - Hooks

//? useState()

/* 
1 Seleccioná la opción correcta:
Los Hooks no pueden ser utilizados dentro de componentes de clase.

2 ¿Para qué sirve el Hook useState()?
useState() sirve para manejar el estado de un componente.

3 Seleccioná la opción correcta:
El único argumento para el Hook useState() es el estado inicial.
*/

//? useEffect()

/* 
1 Anteriormente, los componentes en React, cuando usaban class, permitían que se ejecutara determinada funcionalidad en las distintas etapas que pasaban durante su ciclo de vida (es decir, en la fase de montaje, de actualización y desmontaje). Ahora, si usamos Hooks, también podemos acceder a ese ciclo de vida de una forma más clara y sencilla. ¿Qué Hook nos brinda este beneficio?
useEffect()

2 Seleccioná la opción correcta:
useEffect() recibe dos argumentos. El primero será un callback y el segundo un array.

3 ¿Qué pasa si como segundo argumento pasamos un array vacío?
Le indicamos al Hook que no queremos que le haga seguimiento a ninguna dependencia y, por lo tanto, se ejecutará una sola vez, es decir, cuando el componente se monta.
*/

//? useRef()

/* 
1 ¿Para qué utilizamos el Hook useRef?
Nos permite seleccionar un elemento del DOM.

2 Seleccioná la opción correcta:
Usando el Hook useRef se evita la mutación de elementos DOM.
*/