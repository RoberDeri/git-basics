# Manipulación de repositorios en Git

Este repositorio es una guía de comandos de manipulación con la que poder empezar a trabajar en Git. Previo a comenzar verifique si ha realizado la [instalación y configuración de Git](https://github.com/RoberDeri/git-config) y si dispone de una distribución Linux.
## Creación de un repositorio
Vamos a crear un repositorio nuevo como ejemplo y lo llamaremos "dpl": 

<ol>
  <li>Use el comando <strong>mkdir</strong> para crear directorio y <strong>cd dpl</strong> para entrar en él.</li>
  <li>Inicie con <strong>git init</strong>.</li>
  <li>Se muestra su contenido organizado con <strong>ls -la</strong>.</li>
</ol>

## Comprobar estado de repositorio

<ol>
  <li>Se comprueba con <strong>git status</strong>.</li>
  <li>Cree un fichero llamado "indice.txt" con <strong>cat > indice.txt</strong>. En él, añada la siguiente información:<br><br>
    <ul>
      <li>Capítulo 1: Instalación de Git por el alumno XXX (donde XXX es el nombre del alumno)</li>
      <li>Capítulo 2: Flujo de trabajo básico</li>
    </ul><br>
  </li>
  <li>Confirme con <strong>Ctrl + D</strong>.</li>
  <li>Compruebe estado de nuevo añada el fichero a la zona de intercambio temporal con <strong>git add indice.txt</strong>.</li>
  <li>Repita  <strong>git status</strong> para verificación final.</li>
</ol>

## Realización de commits

Esta es la parte en la que se inicia el seguimiento de los archivos en proceso. Para comenzar, escriba este comando para comenzar el rastreo y añadir un mensaje:<br>

```
git commit -m "Añadido índice de la asignatura DPL."
```

Compruebe con <strong>git status</strong> si se ha registrado este cambio.

## Modificación de ficheros

Modifique el fichero indice.txt con:
```
cat > indice.txt
```

Introduzca los siguientes apartados y una vez hecho confirme con Ctrl + D:
<ul>
  <li>Capítulo 3: Gestión de ramas</li>
  <li>Capítulo 4: Repositorios remotos</li>
</ul><br>
Para mostrar los cambios con respecto a la última versión guardada en el repositorio introduzca:

```
git diff
```
Una vez verificado hacemos commit con el mensaje "Añadido los capítulos 3 y 4":

```
git add indice.txt
git commit -m "Añadido los capítulos 3 y 4"
```
## Consultar historial
El comando <strong>git show</strong> muestra los últimos cambios en el repositorio. El comando <strong>git commit --amend</strong> es una manera práctica de modificar el commit más reciente. Te permite combinar los cambios preparados con el commit anterior en lugar de crear un commit nuevo.

```
git show
git commit --amend -m "Añadido el capítulo sobre gestión de ramas al índice."
```

Escriba git show de nuevo para la comprobación final.



