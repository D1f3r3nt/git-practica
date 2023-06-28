# Practica de Git y Github

## ¿Qué comando utilizaste en el paso 11? ¿Por qué?

> git reset --hard head~1

Se uso este comando porque, de esta manera podemos volver al commit anterior sin que nos queden cambios en el *working copy*

## ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

> git reflog  
> git reset --hard 69637a9

En primer lugar miraremos el historial al completo con "reflog", una vez localizado el commit que queramos restaurar haremos un "reset --hard" para recuperarlo y sin cambios en el *working copy*

## El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, porque no hay cambios en los mismos fragmentos de codigo, ademas se mergea la rama (main) de la cual se a creado la nueva rama (styled) y la rama (main) no ha sufrido ningun commit, por lo tanto tambien es imposible que haya conflictos.

## El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si, porque hay cambios en los mismos fragmentos de codigo, por lo tanto salta un conflicto para que el usuario decida que cambio quiere coger.


## El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, porque no hay cambios en los mismos fragmentos de codigo, ademas en este caso se ha hecho un merge de fast-forward, ya que la rama main ha avanzado hasta donde esta la rama styled asoliendo todos sus commits.

## ¿Qué comando o comandos utilizaste en el paso 25?

> git log --graph

## El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Por poder, puede ser fast-forward o no, todo dependera si queremos que el merge coja todo el recorrido que ha hecho la rama de title, o que salte todo ese recorrido y simplemente genere el resultado del merge de la rama title.

La principal diferencia es que (si es fast-forward) despues la rama main podra retroceder hacia un commit que se haya hecho dentro de la rama title, y el otro caso (si es no-fast-forward) la rama main no podra volver a un cambio de la rama title, ya que en la rama main solo hay el resultado del merge.

Otra diferencia seria que si hacemos fast-forward es imposible tener un conflicto y si hacemos un no-fast-forward hay la posibilidad de que haya un conflicto o no

## ¿Qué comando o comandos utilizaste en el paso 27?

> git reflog  
> git reset a928671


## ¿Qué comando o comandos utilizaste en el paso 28?

> git restore git-nuestro.md

## ¿Qué comando o comandos utilizaste en el paso 29?

> git branch -D title

## ¿Qué comando o comandos utilizaste en el paso 30?

> git reflog  
> git reset --hard e71d574

## ¿Qué comando o comandos usaste en el paso 32?

> git log  
> git checkout 04f036d0


## ¿Qué comando o comandos usaste en el punto 33?

> git log  
> git checkout e71d5744
