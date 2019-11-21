# ¿Qué comando utilizaste en el paso 11? ¿Por qué?
  - git reset --hard HEAD~1, por que este comando me permite volver al commit anterior
    perdiendo los cambios en el working copy
# ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
  - git reset --hard `id commit`, por que con este comando puedo moverme al id commit que especifique
# El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
  - No, porque las dos ramas forman una lista, entonces la rama(master) tiene su HEAD y puntero en el
    ultimo y en este caso unico commit, por lo que creamos rama (styled) y movemos HEAD a esta 
    nueva rama, al hacer merge (master) como esta tiene limpio el "working copy" no nos crea 
    ningun conflicto, lo unico que sucede es que master se actualiza con (styled) 
# El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
  - Si, en este caso si ya que anteriormente este mismo archivo habia sido modificado por (styled),
    por lo que al intentar modificar este mismo archivo con otra rama que se encuentra en la misma
    linea y querer absorber esta rama con (styled),git nos obliga a resorver el conflicto de ambas
    modificaciones.
# El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
  - No, ya que al haber resuelto el conflicto anterior, se puede realizar un merge fast forward 
    ya que como en el caso del paso 13 lo uniico que hace es actualizar su puntero
    y absorber las modificaciones que se hicieran en (styled)
# ¿Qué comando o comandos utilizaste en el paso 25?
  - Hago diagrama de flujo con el comando (git log --graph).
# El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
  - Si, por que la nueva ramificacion (title) se encuentra en la misma linea, el "working copy" de
    master esta limpio por lo que al hacer un commit con (title) y absorber esta rama con master 
    lo que hace el puntero y el HEAD es actualizarse con (title) y absorber las modificaciones. 
# ¿Qué comando o comandos utilizaste en el paso 27?
  - El comando (git reset HEAD~1), para no perder los cambios en el "working copy".
# ¿Qué comando o comandos utilizaste en el paso 28?
  - El comando (git checkout `nombre echivo`)
# ¿Qué comando o comandos utilizaste en el paso 29?
  - Utilizo el comando  (git branch -d `nombre de rama`).
# ¿Qué comando o comandos utilizaste en el paso 30?
  - He utilizado primero (git reflog), con esto consigo todos los id y a continuacion
   (git reset --hard `id commit`)
# ¿Qué comando o comandos usaste en el paso 32?
  - El comando (git reflog) y (git reset `id commit`).
# ¿Qué comando o comandos usaste en el punto 33?
  - El comando (git checkout master), para volver al ultimo commit donde deje el HEAD.