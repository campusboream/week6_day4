# Closures, call, apply y bind

- Dado el siguiente código:

```
function fn() {
    privateMethod(num1, num2) {
        return num1 + num2;
    }

    publicMethod(arg1, arg2) {
        console.log(privateMethod(arg1, arg2));
    }
}
```

Utiliza tus conocimientos sobre closures para que la función fn() retorne el método público y que luego puedas invocarlo para que devuelva por consola la suma de dos números cualesquiera.

- Dada la siguiente clase:

```
class Logger {
    log() {
        console.log(this.fetch);
    }
```

Teniendo en cuenta que la función fetch está definida en el objeto window y que la clase Logger de manera natural no tiene acceso a él, utiliza las funciones call y bind al llamar a la función log() para que el resultado NO sea undefined.

- Dados los siguientes datos:

```
var array = [1,2,3];

class AddValues {
    add() {
        var sum = 0;
        for(var i = 0; i < arguments.length; i++) {
            sum = sum + arguments[i];
        }
        console.log(sum);
    }
}
```

Instancia la clase AddValues y utiliza la función apply para que al llamar a add() con el array de números salga por consola el resultado de la suma de los mismos. Necesitas usar la función apply, que recibe como primer argumento un contexto (que en este caso puede ser null porque no se necesita ninguno en especial) y que recibe como segundo argumento un array de argumentos.

}

# Modules

Los siguientes ejercicios hay que hacerlos dentro de la carpeta es6:

Dentro de esta carpeta encontramos un archivo package.json y un archivo webpack.config.js. Explicamos muy por encima cada uno:

- En el fichero package.json está listada la información del proyecto. De entre toda esa información nos interesan dos cosas:

  - por un lado tenemos la lista de dependencias (la que nos interesa es jquery). Para instalarlas, tenemos que lanzar el comando npm install en la raíz del proyecto.
  - por otro lado, tenemos un script start, que tendremos que lanzar en la raíz del proyecto cuando queramos trabajar (npm start). Este nos servirá un html (el index.html que hay dentro de src) en el localhost:8080. Si accedemos podremos ver la página preparada para este ejercicio. Este html también importa un javascript, que no es otro que el index.js que hay dentro de la carpeta src/js.

- El archivo de webpack contiene una configuración que es necesaria para crear el html final que se sirve en el localhost y además nos permite utilizar los imports de es6.

Dentro de la carpeta src encontramos un archivo index.html con un sencillo template y una carpeta js, que contiene dos archivos:

- el index.js que está casi vacío y tendréis que poblar vosotros,
- el service.js, que ya tiene algunas funciones definidas, aunque dos las tendréis que completar. Especial atención al uso de jQuery.

Según vayáis guardando los cambios en los archivos después de haber lanzado el comando npm start en la terminal, se irán mostrando automáticamente en la página que podéis visitar en localhost:8080.

Todos los ejercicios hay que hacerlos tanto usando los módulos de es6 como los modulos de CommonJS.

Los ejercicios son los siguientes:

- Importar las funciones del service.js en el index.js y utilizarlas para cambiar el título de la segunda noticia y la foto de la tercera noticia utilizando jQuery. Para ello tendréis que importar jQuery y utilizar sus funciones.

- Crear un archivo service-2.js y crear una función que utilice jQuery para escribir una lista de palabras (las que queráis, pero que sean más de dos) utilizando como base la etiqueta "ul" que hay en el html.

# PLUS

- En el index.js tenemos una función llamada renderCount que de momento no hace nada. En el service tenemos una función llamada increment que tampoco hace nada todavía. Hay que completar la función renderCount para que renderice el número de la propiedad count del objeto en el span con clase "count" y para que ese número vaya incrementando cada vez que hacemos click en el botón de al lado. Para ello debéis utilizar y completar la función increment del service. También podéis crear todas las funciones auxiliares que necesiteis.
