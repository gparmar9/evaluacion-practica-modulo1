Para proteger la rama main se ha creado una regla de protección para la rama con las siguientes opciones:

- Require a pull request before merging
- Require approvals (en caso de que haya revisores)
- Require status checks to pass before merging
- Do not allow bypassing the above settings


Es recomendable proteger la rama principal en un proyecto real para evitar un push directo que pueda afectar a la versión de producción, saltarse la revisión, crear bugs entre otras cosas que afecten a la versión final del código. 

Se ha añadido .gitignore para ignorar ficheros con la extensión .log y el contenido de la carpeta __pycache__, esto suelen ser archivos de depuración que se generan cuando se ejecuta código.

- Enlace al repositorio GitHub: https://github.com/gparmar9/evaluacion-practica-modulo1

- Explicación breve del flujo de trabajo: He usado la metodología de trabajo GitHub Flow, donde comenzamos con una rama main protegida, trabajando mediante Pull Requests para cada cambio tras pasar una revisión automática de GitHub. He creado una rama feature para mejora del repositorio y una rama fix para cada cosa que quería arreglar (aunque no lo haya puesto en la documentación)

- El conflicto se produjo en el fichero python operations.py cuando al intentar mergear la rama resta a main después de mergear la rama suma. Había código que se machacaba por lo que he hecho un git merge main a la rama de resta y he modificado el código manualmente para solucionarlo.

- Se utilizado un workflow manual con Github actions para imprimir por la consola el nombre que se le da al action como input.