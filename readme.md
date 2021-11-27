¿Qué comando utilizaste en el paso 11? ¿Por qué?

`git reset --hard` HEAD~1 

He utilizado este comando (que es como utilizar git reset HEAD~1 y git restore*) que vuelve al comit anterior y posteriormente restaura los archivos de mi wokirng copy con el los del commit anterior por lo tanto revierte los cambios hechos.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

Para volver al commit que hemos desecho, utilizamos git reflog. Vemos la referencia del commit y con git reset para movernos con HEAD y la rama styled con el id del commit hasta el otra vez.

Y git restore para recuperar el archivo con los cambios de ese commit.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No porque styles tenia ya acceso a los commits.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Si por que habia modificaciones en las mismas lineas.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No hay conflicto. Hace un merge fast-forward.

**¿Qué comando o comandos utilizaste en el paso 25?**

git log --graph

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

si es de master absorve a title si podria ser fast forwatd porque estan en linea. Pero lo han pedido no fast forward.

**¿Qué comando o comandos utilizaste en el paso 27?**

git reset HEAD~1 para volver al padre de master. 

**¿Qué comando o comandos utilizaste en el paso 28?**

Para descartar cambios usamos git restore <file>

**¿Qué comando o comandos utilizaste en el paso 29?**

 git branch -D title

**¿Qué comando o comandos utilizaste en el paso 30?**

primero usamos git reflog para saber el id del commit al que ir y luego git reset

**¿Qué comando o comandos usaste en el paso 32?**

primero usamos git reflog para saber el id del commit inicial y luego git reset

**¿Qué comando o comandos usaste en el punto 33?**

Primero usamos git reflog para saber el id del commit al que ir y luego git reset
