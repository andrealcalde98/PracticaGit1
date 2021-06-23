- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
 
git reset --hard HEAD~1
Usamos este comando para deshacer los cambios del último commit, 
este nos permite también perder los cambios en el working copy.
Por lo tanto perdemos los cambios del punto 9).
 
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

git reflog -> Para conocer el historial de commits y saber a donde
regresar con el codigo corresponiente.
git reset --hard "codigo" -> para regresar al commit anterior.
  
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 

Nos indica que ya esta al dia porque la rama actual "styled "contiene todo
el contenido de "master".

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?  

Genera conflictos ya que "styled" no tiene los últimos cambios de "htmlify"
por lo tanto te pide que los revises antes de continuar.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?  

No causo ningun conflicto, aplicó los cambios de la rama "styled"
ya que "styled" contenia todos los cambios de "master", entonces
procede a compartir sus cambios y aplicarlos en "master".

- ¿Qué comando o comandos utilizaste en el paso 25?  

Usamos el comando siguiente: git log --pretty=oneline --graph
este nos pinta una pequeña grafica de los commits hechos.

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

Si es possible ya que la rama "title" parte de la rama "master"
por lo tanto "master" puede obtener solo los cambios de "title"
sin generar ningun conflicto.

- ¿Qué comando o comandos utilizaste en el paso 27? 

He usado git reset HEAD~1, usamos este comando para retroceder un paso
sin el --hard para no perder los cambios en el working copy.

- ¿Qué comando o comandos utilizaste en el paso 28? 

Para descartar los cambios hacemos un git checkout "documento"
así volvemos el HEAD hacia el documento sin los últimos cambios
por lo tanto los cambios quedan descartados.

- ¿Qué comando o comandos utilizaste en el paso 29? 

Borramos la rama "title" con git branch -D title.

- ¿Qué comando o comandos utilizaste en el paso 30? 

Tal y como hemos hecho en el paso 12, hacemos un git reflog para
obtener el codigo del merge hecho anteriormente, luego hacemos un
git reset --hard "codigo" para rehacer el merge y colocarnos en
ese punto.

- ¿Qué comando o comandos usaste en el paso 32? 

Volvemos a usar reflog para opbtener el código del primer commit
y usamos git reset --hard "codigo" para volver al commit iniciar.

- ¿Qué comando o comandos usaste en el punto 33? 

Volvemos a usar reflog y también git reset --hard "codigo" 
para volver a la última modificación.