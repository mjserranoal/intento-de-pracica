# Práctica de git María José Serrano Alcántara.

- **11**.  git reset --hard HEAD~1
He utilizado este comando puesto que quería deshacer el último cambio y, además, eliminarlo del woeking copy utilizando así el parámetro -- hard. He añadido el puesto número 1 ya que quería mover el HEAD  una sola posición atrás.

- **12**. Primero, he hecho un git reflog para buscar el sha del commit anterior, después he utilizado git reset <sha del commit anterior> y, por último, he ejecutado un git restore git-nuestro.md para restaurar los cambios del archivo.

- **13**. No se han producido conflictos puesto que al crear la rama styled de la rama master ésta ya contenía todos los commits existentes en master ya que no hemos añadido ningún commit nuevo desde que styled se creó.

- **19**. Sí, se produce conflictos puesto que hemos hecho un cambio en el archivo <git-nuestro> en la rama htmlify y al ser absorvido ese commit por <styled> detecta cambios en las mismas líneas del archivo y nos pregunta con qué información debe quedar el archivo.

- **21**. No, puesto que no ha habido commits en master que modifiquen el archivo desde que se creo styled y, por lo tanto, al tener styled los commits que hay en master puede traerse los commits de styled con un fast-forward ya que no hay riesgo de que se pierda información.

- **25**. 
    + git log –graph

- **26**. Si, podría ser un fast forward ya que la rama title no tendría conflictos con la rama master al absorber esta sus commits.

- **27**. 
    + git reset HEAD~1

- **28**.
    +  git checkout 
    + git-nuestro.md

- **29**. 
    + git branch -D title.

- **30**. 
    + git reflog
    + git reset <SHA del commit del merge>
    + git restore git-nuestro.md

- **32**.
    + git reflog
    + git reset <sha del primer commit>

- **33**. 
    + git reflog
    + git reset <sha del commit donde pusimos el título al poema>