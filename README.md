# Manipulación de repositorios en Git

Este repositorio es una guía de comandos de manipulación con la que poder empezar a trabajar en Git. Previo a comenzar verifique si ha realizado la [instalación y configuración de Git](https://github.com/RoberDeri/git-config) y si dispone de una distribución Linux.
## Creación de un repositorio
Vamos a crear un repositorio nuevo como ejemplo y lo llamaremos "dpl": 

<ol>
  <li>Use el comamdo <strong>mkdir</strong> para crear directorio y <strong>cd dpl</strong> para entrar en él.</li>
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
  <li>Confirme con <strong>Ctrl +D</strong>.</li>
  <li>compruebe estado de nuevo añada el fichero a la zona de intercambio temporal con <strong>git add indice.txt</strong>.</li>
  <li>Repita  <strong>git status</strong> para verificación final.</li>
</ol>

## Modificación de ficheros
