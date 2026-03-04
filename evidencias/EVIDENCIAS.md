Para proteger la rama main se ha creado una regla de protección para la rama con las siguientes opciones:

- Require a pull request before merging
- Require approvals (en caso de que haya revisores)
- Require status checks to pass before merging
- Do not allow bypassing the above settings


Es recomendable proteger la rama principal en un proyecto real para evitar un push directo que pueda afectar a la versión de producción, saltarse la revisión, crear bugs entre otras cosas que afecten a la versión final del código. 