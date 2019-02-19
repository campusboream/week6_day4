# Closures, call, apply y bind

- Crea una función que devuelva un array1 con los números primos contenidos en otro array2 de números del 1 al 20. El array2 debe ser privado y no modificable desde fuera de la función.

- Dada la siguiente función:

```
function showTotalValue(val1, val2, val3) {
    console.log(val1 + val2 + val3 + this.val4 + this.val5);
}
```

utiliza la función call para que el valor que salga por consola sea igual a 25. Luego haz lo mismo pero utilizando las funciones apply y bind.

# Modules

Estos ejercicios hay que hacerlos dentro de la carpeta es5

- Crear un archivo service.js y declarar en él una función que admita como argumento un array de 10 palabras y que retorne otro array que contenga solo las palabras que empiecen por la letra 'a' del primer array y exportar la función. Luego crear un archivo index.js desde el cual importar la función y utilizarla para sacar por consola el array reusltando.

Los siguientes, hay que hacerlos dentro de la carpeta es6:

Dentro de esta carpeta encontramos un archivo package.json y un archivo webpack.config.js. Explicamos muy por encima cada uno:

- En el fichero package.json está listada la información del proyecto. De entre toda esa información nos interesan dos cosas:

  - por un lado tenemos la lista de dependencias (la que nos interesa es jquery)
  - por otro lado, tenemos un script start, que tendremos que lanzar cuando queramos trabajar. Este nos servirá un html (el index.html que hay dentro de src) en el localhost:8080. Si accedemos podremos ver la página preparada para este ejercicio. Este html también importa un javascript, que no es otro que el index.js que hay dentro de la carpeta src/js.

- El archivo de webpack contiene una configuración que es necesaria para crear el html final que se sirve en el localhost y además nos permite utilizar los imports de es6.

Dentro de la carpeta src encontramos un archivo index.html con un sencillo template y una carpeta js, que contiene dos archivos: - el index.js que está vacío y tendréis que poblar vosotros, - el service.js, que ya tiene un par de funciones definidas, aunque una de ellas la tendréis que completar. Especial atención al suo de jQuery.

El ejercicio es el siguiente:

- Importa las funciones del service.js en el index.js y utilízalas para cambiar el título de la segunda noticia y la foto de la tercera noticia. Si no funcionan, averigua que falta en el archivo service.js

- Crea un archivo service-2.js y crea una función que utilice jQuery para escribir una lista de palabras (las que queráis, pero que sean más de dos) utilizando como base la etiqueta <ul> que hay en el html.

Según vayáis guardando los cambios en los archivos después de haber lanzado el comando npm start en la terminal, se irán mostrando automáticamente en la página que podéis visitar en localhost:8080.
