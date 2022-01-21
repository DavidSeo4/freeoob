# Creación de la estructura de un sitio web con Bootstrap/Sass/Parcel.

1. Para comenzar creamos la estructura del sitio web e incluimos e instalamos bootstrap y el manejador de paquetes desde la consola con los siguientes códigos:

- npm init -y

- npm install --save-dev parcel-bundler sass

-  touch scss/style.scss

-  touch .sassrc

- touch src/index.html

  ![image-20220120145033952](C:\Users\Usuario\AppData\Roaming\Typora\typora-user-images\image-20220120145033952.png)

2. A medida que creamos los archivos como por ejemplo Index.html los rellenamos con el código dado con el fin de ir configurando el sitio web.

3. A continuación instalamos Popper, nuevamente desde la consola, con el código " npm install @popperjs/core". También creamos el index.js que nos permitirá posteriormente validar el formulario y le añadimos "import * as bootstrap from 'bootstrap';" en la primera linea para conectar el JS con Bootstrap.

4. Con el fin de comprobar como va el proyecto añadimos la linea de código " "start": "parcel ./src/index.html"," dentro de package.json e introducimos "npm start" en la consola. Esto pondrá en marcha el servidor y nos peritira ver el estado del sitio web.

   ![image-20220120144941089](C:\Users\Usuario\AppData\Roaming\Typora\typora-user-images\image-20220120144941089.png)

5. Adaptamos nuestra hoja de estilos a Bootstrap añadiendo en el código de la misma los siguientes "imports":

   1. @import "../node_modules/bootstrap/scss/functions";
   2. @import "../node_modules/bootstrap/scss/variables";
   3. @import "../node_modules/bootstrap/scss/mixins";

6. Para acabar este punto, creamos o introducimos el formulario que consideremos necesario en el index.html y creamos un nuevo archivo js en el que introducimos la validación para este mismo formulario. Una vez todo está enlazado correctamente dentro del index.html la página debería ser funcional y mostrar un formulario validable dentro de http://localhost:1234 .

7. El siguiente paso consiste en crear un archivo php con el fin de recoger los datos que introducimos en el formulario. Para ello creamos el archivo login_basico.php e introducimos los echos correspondientes con los valores que solicitamos en el formulario.

![image-20220121100314380](C:\Users\Usuario\AppData\Roaming\Typora\typora-user-images\image-20220121100314380.png)

7. Ahora editamos en Index.html enlazando los apartados correspondientes con el archivo php. Lo que añadimos será:

   1. "name" y su valor en los inputs de cada apartado.

   2. "action" al inicio del formulario para enlazar el archivo php al mismo.

   3. "method= "post" para que nos muestre la información en pantalla una vez validamos el formulario. 

      ![image-20220121100244317](C:\Users\Usuario\AppData\Roaming\Typora\typora-user-images\image-20220121100244317.png)

8. Reiniciamos el servidor desde la consola escribiendo nuevamente npm start y al rellenar el formulario y pulsar enviar debería mostrar un listado con las secciones rellenadas y sus valores.

![image-20220121104159289](C:\Users\Usuario\AppData\Roaming\Typora\typora-user-images\image-20220121104159289.png)

