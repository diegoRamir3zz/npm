<h2 style="text-align: center;">
My notes <img src="https://img.icons8.com/windows/32/000000/npm.png"/>
</h32>


<h3>Empezando un proyecto</h3>
<p>
Hay dos maneras de empezar un proyecto con npm

1. Llenando todos los datos inmediatamente, con el comando <i><b>npm init</b></i> de esta manera le introducimos los datos que npm necesita.
2. Iniciando un proyecto rapido con datos ya establecidos. Utilizamos el comando <i><b> npm init -y</b></i> asi npm llenara los datos automaticamente.

<i><b>Establecer datos predeterminados </b></i>

  <i> npm set init.author.email "(EMAIL)"</i><br>
  <i>npm set init.author.name "(NAME)"</i><br>
  <i>npm set init.license "(LICENSE)"</i><br>
  ** Sin los parentesis.
</p>

<h3>Instalando dependencias</h3>

<p>
<i><b>Formas de instalar dependencias</b></i>

1. <i><b>npm install (nombreDependencia)</b></i> este comando instala la dependecia como parte de nuestro proyecto, solo en la carpeta del mismo
 <i>shortcut:<b> npm i (nombreDependencia) -S</b></i>

2. <i><b>npm install (nombreDependencia) --save-dev</b></i> este comando instala la dependecia como desarrollo solo en nuestro proyecto
  <i>shortcut:<b> npm i (dependencie) -D</b></i>

 <b>NOTA:</b> Es bueno tener presente que dependencias mandamos al repositorio y cuales no. Por ejemplo, debemos evitar enviar nuestra carpeta de node_modules.
 <i>Para no enviar la carpeta node_modules a nuestro repositorio escribimos en nuestro archivo .gitignore lo siguiente: <b>node_modules/</b></i>

3. Instalar dependencias de forma global

  <i>comando: <b>sudo npm install -g (nombreDependencia)</b></i><br>
   <i> shortcut: <b>sudo npm i -g (nombreDependencia)</b></i>
  Para saber si un paquete se intalo de manera global utilizamos el siguiente comando <i><b> npm list -g --depth 0</b></i>

4. instalar dependencias de forma opcional

  <i>comando:<b> npm install (nombreDependencia) -O </b></i>

5. ver el output de la dependencia

  Para ver cuantos archivos instalará una dependecia, sin que la instale utilizamos el siguiente comando:<i><b> npm install (nombreDependencia) --dry-run </b></i>

6. forzar una instalación 

 <i> comando: <b>npm install (nombreDependencia) --force</b></i>
   <i> shortcut: <b>npm i (nombreDependencia) -f</b></i>

7. Instalar una versión espesifica

  <i>comando: <b>npm install (nombreDependencia@versión)</b></i>
</p>

<h3>Actualizar dependencias</h3>
<p>
1. Verificar que dependencias necesitas actualización

  <i>comando:<b> npm outdate</b></i>
  Si queremos que procesos realiza npm podemos utilizar el siguiente comando:  <i><b>npm outdate --dd</b></i>

 2. Actualizar una dependencia 

  <i>comando:<b> npm update</b></i>. Para instalar la ultima versión de una dependencia en espesifico utilizamos el siguiente comando:<i><b> npm install (dependencie@latest)</b></i>

 3. Eliminar dependencias

    <i>comando: <b>npm uninstall (dependencie)</b></i> Para eliminar la dependencia solo de node_modules pero NO del package.json utilizamos el comando<i><b> npm uninstall (dependencie) --no-save</b></i>

4. Simbolos

  En el package.json se encuentran las versiones de las dependencias que tenemos instaladas.

  <i><b>Como funcionan las versiones</b></i>
 <i>ejemplo: </i> version 1.15.0
  1 = cambio mayor,
  15 = cambio medios,
  0 = cambios menores.

 <i><b>El caret (^) </b></i>Si este simbolo esta en donde se espesifica la version de la dependencia, significa que permite las actualizaciones de dicha dependencia.

Si le quitamos el caret (^) Le indicamos que no queremos que actualice la dependencia
</p>