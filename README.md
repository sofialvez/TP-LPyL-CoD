# TP - Laboratorio de Programación y Lenguajes del grupo "Code of Duty"

## Integrantes: 
Alvez, Sofía.  
Maldonado, Ignacio.  
Mentoro, Facundo.  
Romero, Sergio.  

## Descripción: 

Api desarrollada en Node.js y Express.js utilizando Middlewares, Controladores, Schemas, Migrations Models y Routes.  
El objetivo y funcionamiento de la misma es controlar una base de datos, haciendo Get, Post, y Delete.
Tiene una base de carreras, donde cada carrera tiene sus materias.   
Una carrera tiene muchas materias, y cada materia solo se encuentra en una carrera.  

## Guia de Instalación:

### Opcion 1 - Clonacion de Repositorio (HTTPS).  
 
Desde la terminal Git Bash ir al directorio donde se desea clonar el proyecto. Escribir el siguiente comando para clonar el repositorio
**git clone https://github.com/Veik1/TP-LPyL-CoD.git**

###  Opcion 2 - Descarga de Repositorio.

Desde el boton <**Code**> elegir la opcion Download ZIP para descargar el repositorio. Descomprimirlo en el directorio donde se va a deplegar el proyecto

Una vez que se tenga el proyecto en el directorio deseado, en un Simbolo de Sistema (CMD) ir hasta el proyecto y abrir VSCode (code .)

## Intalacion de Dependencias e Inicio del Proyecto
En una terminal dentro de VSCode, correr el siguiente comando para intalar todas las dependencias necesarias para iniciar correctamente el proyecto
	**npm install**
Luego que se intalen todas las dependecncias, para iniciar el servidor del proyecto correr el siguiente comando:
	**npm run dev**


## Uso y Pruebas en Postman
Una vez intalado y ya corriendo el proyecto en el entorno local..
. Abrir Postman
. En **Collections** ir a Import
. Buscar en files el archivo **“CRUD Testing.postman_collection”** dentro del proyecto

Los resultados de las pruebas deben ser los siguientes: 

**Get**	     /carreras	              Resultado: 200	Obtener todas la carreras   
**Get**	     /carreras/:id	          Resultado: 200, 404	Obtener una carrera en particular   
**Post**	    /carreras	              Resultado: 201 , 400	Crear una Carrera   
**Delete**	  /carreras/:id	          Resultado: 200, 404	Borra una carrera en particular   
**Post**	    /carreras/:id/materia	  Resultado: 201, 404, 400	Crea un materia dentro de una carrera    
**Get**	     /carreras/:id/materias 	Resultado: 200, 404	Obtener todas la materias de una Carrera    
**Get**	     /materias	              Resultado: 200	Obtener todas las materias     
**Get**	     /materias/:id	          Resultado: 200, 404	Obtener una materia en particular     
**Delete**	  /materias/:id          	Resultado: 200, 404	Borra una materia en particular      
