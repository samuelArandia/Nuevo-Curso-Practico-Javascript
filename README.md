# Nuevo curso practico de javaScript

## Variables y operaciones

1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es una variable y para qué sirve?

Es un espacio reservado en memoria que nos permite almacenar información. Podemos almacenar diferentes tipos de datos para usarlos en nuestro código. En JS existe tres formas de crear una variable var, let, const. en ES6 nacen let & const que son variable de tipo scope y esto quiere decir que dependiendo del scope es su accesibilidad.
   
¿Cuál es la diferencia entre declarar e inicializar una variable?

Cuando declaramos una variable, simplemente nombramos la variable, sin indicarle que tipo de información o dato almacenara. En cambio, cuando inicializamos una variable indicamos el tipo de dato e información que va a almacenar.


          // Declara una varibale 
            const nombre 
          // inicializar una variable 
            const nombre = "samuel" 
          
¿Cuál es la diferencia entre sumar números y concatenar strings?

La diferencia es que al sumar numeros estamos haciendo uso del operador matematico (+) para obtener la sustraccion de numeros y al concatenar strings estamos uniedo caracteres utilizado de igual forma el operador 

        // Suma 
          resultado = 2 + 2 
          resutlado = 4 
        // Concatenar 
        resultado("Hola" + "mundo")
       
¿Cuál operador me permite sumar o concatenar?
    
 El operador es + 
    

2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

    Nombre = STRING
    Apellido = STRING 
    Nombre de usuario en Platzi = STRING 
    Edad = NUMBER 
    Correo electrónico = STRING 
    Mayor de edad = BOOLEAN 
    Dinero ahorrado = NUMBER 
    Deudas = NUMBER 

3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.
          
          
          // Variables 
             let nombre = "Samuel"
             let apellido = "Arandia"  
             let nombreUsuarioPlatzi = "samuelArandia"  
             let edad = 25
             let email = "samuelarandia@gmail.com 
             let mayorEdad = true;
             let dineroAhorrado = 10000; 
             let deudas = 15000000;


4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

    Nombre completo (nombre y apellido)
    Dinero real (dinero ahorrado menos deudas)
    
    //Nombre completo 
    let nombreCompleto  = nombre + ' ' + apellido; 
    console.log (nombreCompleto)
    
    // Dinero real 
    let dineroReal = dineroAhorrado - deudas; 
    console.log(dineroReal);
    
    
## Funciones


1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es una función?

Un conjunto de intrucciones que realizan una tarea o calculan un valorm, pero para que un procedimiento califique como funcion, debe tomar alguna entrada y devolver unas salida donde hay una relacion obvia entre la entrada y la salida. 


¿Cuándo me sirve usar una función en mi código?

Cuando tenemos variables o bloquees de código que pueden comportarse como parámetros y argumentos que podemos encapsular para usar más de una vez en el futuro. Y ordenar y hacer mas legible nuestro código.

¿Cuál es la diferencia entre parámetros y argumentos de una función?

Los parámetros son variables a las que se les asignará un valor. 
### <<Las funciones reciben parámetros al redactarse>>

Los Argumentos son los valores asignados a los parámetros al ejecutarse.
### <<Las funciones reciben argumentos al ejecutarse>>
![imagen](https://user-images.githubusercontent.com/83564327/196000641-4b8b78ec-a8c8-460a-9121-e0956802d89d.png)


2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

            const name = "Juan David";
            const lastname = "Castro Gallego";
            const completeName = name + lastname;
            const nickname = "juandc";

              console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
              
            //Funcion
            
            function miNombreCompleto(name, lastname) { 
              return name + " " + lastname 
            }
            functionsaludo(name, lastname, nickname){
              const completeName = nombreCompleto(name, lastname);
              console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname     + ".");
             };


### Condicionales

1️⃣ Responde las siguientes preguntas en la sección de comentarios:

 ¿Qué es un condicional?
 
Un bloque de código que se ejecuta dependiendo de las condiciones establecidas previamente. Para establecer dichas condiciones usamos:
 
¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?

If (else, else if),

Nos permite hacer validaciones de variables distintas en cada condicional (si eso requerimos).

Switch (case),

En cambio usando Switch todos los case se validan con la misma variable o condición previamente definida en Switch .

¿Puedo combinar funciones y condicionales?

Si, las condicionales se pueden encapsular en cualquier bloque de codigo dentro de las funciones.

2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

              const tipoDeSuscripcion = "Basic";
              
              switch (tipoDeSuscripcion) {
                 case "Free":
                     console.log("Solo puedes tomar los cursos gratis");
                     break;
                 case "Basic":
                     console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
                     break;
                 case "Expert":
                     console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
                     break;
                 case "ExpertPlus":
                     console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
                     break;
              }            
              
              // Utilizando if, else, if else
              
              const tipoDeSuscripcion = "Basic";
              
              function CualesTipoDeSuscripcion(tipoDeSuscripcion) { 
                if (tipoDeSuscripcion == "Free") { 
                    console.log("Solo puedes tomar los cursos gratis");
                 } else if (tipoDeSuscripcion == "Basic") { 
                    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes"); 
                 } else if (tipoDeSuscripcion == "Expert") {
                    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
                  } else {
                     console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
                  }
              }

3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

              functiontipoSuscripcion(suscripcion) {
              	if (suscripcion == "Free"){
              	console.log("Solo puedes tomar los cursos gratis");
              	return;
              }if (suscripcion == "Basic") {
              	console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
              return;
              }if (suscripcion == "Expert"){
              	console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
              return;
              }if (suscripcion == "ExpertDuo") {
              	console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
              return;
              }
              console.warn('Este tipo de suscripción no existe')
              };
              
    💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏

         const tipoDeSuscripcion = { 
         free: "Solo puedes tomar los cursos gratis"
         basic: "Puedes tomar casi todos los cursos de Platzi durante un mes"
         expert: "Puedes tomar casi todos los cursos de Platzi durante un año"
         expertduo: "Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"
   }
   
   para ingresar a los objeto puedo ingresar de esta forma: 
   
         tipoDeSuscripcion.free 
         tipodeSuscripcion['free']
         
         function conseguirTipoDeSuscripcion(sucripcion) {
                  if (tipoDeSuscripcion[suscripcion]) {
                     console.log(tipoDeSuscripcion[suscripcion])
                     return;
                  }
                  console.warn('Ese tipo de suscripcion no existe')
            }
   
   
### Ciclos
1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es un ciclo?
Es una estructura de control que nos permite repetir instrucciones una determinada cantidad de veces dependiendo de un iterador o una condición

¿Qué tipos de ciclos existen en JavaScript?

Existen 3 tipos de ciclos: For, while, do while 

¿Qué es un ciclo infinito y por qué es un problema?

Un ciclo infinito es una repetición indeterminada de instrucciones y se da cuando la condición o el iterador no indican cuantas veces se va a repetir, esto provoca que se ejecuten infinitamente, es un problema porque puede llenar la memoria del sistema y provoque un colapso del mismo

¿Puedo mezclar ciclos y condicionales?

Si, por supuesto. 

2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

              for (let i = 0; i < 5; i++) {
                  console.log("El valor de i es: " + i);
              }
              
              let i= 0 
              while(i < 5) { 
                 console.log("El valor de i es: " + i);
                 i++;
              }
              
              
              for (let i = 10; i >= 2; i--) {
                  console.log("El valor de i es: " + i);
              }
              
              let i = 10
              while (i >= 2) {
                  console.log("El valor de i es: " + i);
                  i--;
              }


3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

    💡 Pista: puedes usar la función prompt de JavaScript.
    
          let result;
          
          do {
            result = prompt("Cuanto es 2+2?");
              if(result == 4){
                  console.log("Felicidades, tu conocimiento en matemáticas es avanzado :v");
              }
          } while ( resut != 4);
          

### Listas

1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es un array?

Es una lista de elementos, que pueden estar ordenadas o desordenadas. Ejemplo de array: 
         
         const array = [1,'samuel', true, false, 'Arandia']

¿Qué es un objeto?

Un objeto es una colección de propiedades, y una propiedad es una asociación entre un nombre (o clave) y un valor. El valor de una propiedad puede ser una función, en cuyo caso la propiedad es conocida como un método. Además de los objetos que están predefinidos en el navegador, puedes definir tus propios objetos. Este capítulo describe cómo usar objetos, propiedades, funciones y métodos; y cómo crear tus propios objectos.

Es una lista de elementos pero cada elemento tiene un nombre clave. 

         const obj = {
            nombre:'samuel',
            apellido: 'Arandia',} 

¿Cuándo es mejor usar objetos o arrays?

Los arrays son objetos iterables y se accede a la información a través de un número, si no conocemos la posición de un dato necesitamos recorrer el arreglo para encontrarlo, en cambio en un objeto los datos están enlazados con una llave o un “nombre”, estos objetos no se pueden recorrer y se accede a los datos con la llave

Los arrays se utilizan cuando almacenamos múltiples valores de una sola variable, mientras que un objeto puede contener múltiples variables con sus valores. un array también se puede considerar como un objeto y tiene la mayoría de las funcionalidades del objeto.

¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

Si
![imagen](https://user-images.githubusercontent.com/83564327/196036138-4793f875-b3e1-412e-8dc4-0b6fe231a914.png)

2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

            let arrayNew = ['puerto aysen', 'puerto cisne', 'puerto tranquilo', 'puerto chacabuco'];
             function readArray(array) { 
                  console.log(array[0]);      
             
             }
             readArray(arrayNew);
3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

            let arrayNew = ['puerto aysen', 'puerto cisne', 'puerto tranquilo', 'puerto chacabuco'];
             function readArray(array) { 
                array.forEach(element => console.log(element));
             }        

4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).
¿Cómo te fue? 🏆

                     park = {
                         name: 'patagonia',
                         location: 'Ruta 7',
                         country: 'chile',
                       };
                     
                     function readObject(object) {
                         const array = Object.values(object);
                         for (let i = 0; i < array.length; i++) {
                             console.log(array[i]);
                         }
                     }
                     readObject(park);
                     

¡Felicidades por completar la prueba de JavaScript! Confío en que hayas completado cada paso y hayas pausado para repasar los temas de los ejercicios que se te complicaron.

Ahora sí, continúa a la siguiente clase, pero recuerda que ya no puedes abandonar el curso, debes completarlo hasta el final. No importa cuánto tiempo te tome. Yo sé que tú puedes. Y tú deberías de saberlo también.

¡Te espero en la siguiente clase para comenzar!
