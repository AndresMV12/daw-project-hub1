# DAW Project Hub

Pequeña página web para practicar un flujo profesional de trabajo con Git y GitHub.

## Historial del proyecto

Durante el desarrollo se han realizado varios commits para registrar los cambios de forma ordenada.

Es mejor realizar commits pequeños porque permiten identificar fácilmente los cambios, encontrar errores y recuperar versiones anteriores.

El commit dd2780a añadió los tres párrafos sobre desarrollo web, despliegue y trabajo colaborativo.

## Seguridad y archivos ignorados

El archivo .gitignore permite excluir archivos que no queremos
subir al repositorio, como configuraciones privadas o archivos
temporales.

### Reflexión de seguridad

1. **¿Por qué se puede publicar .env.example?**
Porque contiene únicamente los nombres de las variables,
sin contraseñas ni tokens reales.

2. **¿Por qué debemos ignorar .env?**
Porque puede guardar información privada de la aplicación,
como contraseñas o claves de acceso.

3. **¿Qué hacer si publicamos una contraseña o token real?**
Debemos revocar o cambiar inmediatamente la credencial y
comprobar si alguien ha podido utilizarla.

4. **¿Basta con eliminar el archivo en otro commit?**
No, porque seguirá apareciendo en el historial de Git.
También habría que limpiar las copias del historial donde
aparezca la información.

## Conflicto resuelto

Durante el desarrollo del proyecto se provocó un conflicto
de fusión entre las ramas main y feature/nuevo-eslogan.

El conflicto ocurrió porque ambas ramas modificaron
la misma línea del archivo index.html, concretamente
el párrafo de presentación de la página.

Git no pudo decidir automáticamente qué versión conservar,
por lo que fue necesario resolver el conflicto manualmente.

Para solucionarlo, se redactó un nuevo eslogan que combina
las ideas de las dos ramas.

Después se eliminaron los marcadores del conflicto,
se añadió el archivo con git add y se completó la
fusión mediante un commit.

Finalmente, se comprobó la resolución revisando el
historial de Git y el funcionamiento de la página web.

## Cómo abrir la página

Para abrir la página web debemos descargar o clonar
el repositorio de GitHub.

Después, abrimos la carpeta del proyecto en Visual Studio
Code y ejecutamos index.html con Live Server o directamente
desde un navegador.

La página está desarrollada únicamente con HTML y CSS,
por lo que no necesita instalar dependencias adicionales.

## Actualización desde GitHub

Este apartado se ha añadido directamente desde GitHub
para comprobar cómo funcionan git fetch y git pull.

## Diferencias entre fetch y pull

### ¿Qué hace git fetch?
Descarga los cambios del repositorio remoto, pero no modifica
automáticamente los archivos de nuestra rama local.

### ¿Qué hace git pull?
Descarga los cambios del repositorio remoto y los integra
en nuestra rama local.

### ¿Por qué es útil git fetch?
Porque nos permite revisar las modificaciones antes de
incorporarlas a nuestro trabajo y detectar posibles problemas.

### ¿Qué relación existe entre fetch y pull?
Git pull realiza primero una descarga similar a git fetch
y después integra los cambios mediante merge o rebase.

## Forks y colaboración

### 1. ¿Qué es un fork en GitHub?
Un fork es una copia de un repositorio que se crea en nuestra
cuenta de GitHub para poder trabajar en él sin modificar
directamente el proyecto original.

### 2. ¿En qué se diferencia un fork de una rama?
Una rama es una línea de desarrollo dentro de un repositorio.
Un fork es otro repositorio independiente, aunque está
relacionado con el original.

### 3. ¿En qué cuenta se almacena un fork?
Normalmente se almacena en la cuenta de GitHub de la persona
que lo crea.

### 4. ¿Cuándo es útil trabajar mediante un fork?
Cuando queremos colaborar en un proyecto de otra persona
sin tener permisos para modificar directamente su repositorio.

### 5. ¿Qué relación existe entre el repositorio original y el fork?
El fork parte del repositorio original, pero después puede
tener cambios diferentes. Ambos pueden seguir evolucionando.

### 6. ¿Qué es el repositorio upstream?
Es el repositorio original del que procede nuestro fork.
Podemos utilizarlo para consultar y descargar sus cambios.

### 7. ¿Qué diferencia existe entre origin y upstream?
Origin suele identificar nuestro repositorio remoto.
Upstream suele identificar el repositorio original
del que hemos creado el fork.

### 8. ¿Cómo enviamos cambios del fork al repositorio original?
Podemos crear una pull request para proponer que los
responsables del proyecto incorporen nuestras modificaciones.

### 9. ¿Quién decide si se acepta la propuesta?
Los responsables del repositorio original, después de
revisar los cambios realizados.

### 10. ¿Puede seguir evolucionando el repositorio original?
Sí. El repositorio original puede recibir nuevos commits
aunque existan forks creados por otros desarrolladores.