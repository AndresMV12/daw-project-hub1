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