# REST API Primeros pasos


// iniciar proyecto node.js

*npm init -y*   // Se crea el package.json

// instalar typescript local si no se instaló global

*npm i typescript --save-dev*         //Local

*npm i typescript -g*                 //Global

// Iniciar proyecto typescript

https://medium.com/@bhagyamangale/tsc-init-4665ec9d7b09

*tsc --init*                         //Si global. Se crea el tsconfig.json

*npx tsc --init*                     //Si local. Se crea el tsconfig.json

*git init*                            // Para crear el repositorio local

// Cambiamos la configuración del *tsconfig.json*

*"target": "es6",*

*"outDir": "./build",*

// Instalación de express, mongoose y morgan

https://dev.to/mtee/getting-started-with-morgan-3d1m

// Morgan is a middleware function for logging information 

// about the http request/response in a server application.

// Un middleware es un bloque de código que se ejecuta entre 

// la petición que hace el usuario (request) hasta que la petición llega al servidor.

*npm i express mongoose morgan*

// nodemon is a tool that helps develop node.js based 
// applications by automatically restarting the node 
// application when file changes in the directory are detected.

// Instalamos los tipos de datos y módulos de desarrollo

npm install @types/node @types/mongoose @types/express @types/morgan nodemon typescript -D


// Configuramos el *.gitignore* con:
// ATENCION NO PONER build si subimos a heroku
*node_modules*

// Creamos la carpeta *src* con *server.ts*   //Archivo typescript

//Con el contenido que presentamos

// Cambiamos el package.json con:

  "scripts": {

    "ts": "tsc -w",

    "dev": "nodemon ./build/server.js",

    "start": "node ./build/server.js"

  },

  // Para compilar
  
  *npm run ts*  // que como tiene el -w incorporado se compilará si cambiamos el código
  
  // Para ejecutar en desarrollo
  *npm run dev*  // que como tiene el nodemon se reiniciará el servidor si cambiamos
                // además como tenemos 
  
  // Para ejecutar en producción
  *npm start*

  // Ya podemos invocar con localhost:3000

  y vemos el log:

  PS C:\Users\Adolfo3\Documents\ACurso2021\ASGBD\ProyectosTS\restapitriangulo000> npm run dev

> restapitriangulo000@1.0.0 dev 

C:\Users\Adolfo3\Documents\ACurso2021\ASGBD\ProyectosTS\restapitriangulo000

> nodemon ./build/server.js

[nodemon] 2.0.6

[nodemon] to restart at any time, enter `rs`

[nodemon] watching path(s): *.*

[nodemon] watching extensions: js,mjs,json

[nodemon] starting `node ./build/server.js`

Server on port: 3000

[nodemon] restarting due to changes...

[nodemon] starting `node ./build/server.js`

Server on port: 3000

GET / 404 1.984 ms - 139

--


git init

git add .

git commit -m "primer commit"

git branch -M rama001   // Escogemos el nombre de la rama

git remote add origin https://github.com/asalsan790/restapitriangulo000.git

git push -u origin rama001  // hacemos push de nuestra rama.



//Para ver a donde apunta cada rama

git log --oneline --decorate

// Crear una nueva rama

git branch rama002

// Cambiar de rama

git checkout rama002

git add .

git commit -m "en nueva rama"

git push -u origin rama002   


--
