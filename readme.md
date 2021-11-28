**¿Qué comando utilizaste en el paso 11? ¿Por qué?**

git reset --hard HEAD~1 

He utilizado este comando (que es como utilizar git reset HEAD~1 y git restore*) que vuelve al commit anterior y posteriormente restaura los archivos de mi wokirng copy con el los del commit anterior por lo tanto revierte los cambios hechos.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

Para volver al commit que hemos desecho, utilizamos git reflog. Vemos el id del commit y con git reset movemos el HEAD y la rama styled a ese commit otra vez. 
Y después git restore para recuperar el archivo como estaba en ese commit.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No porque la rama styles(que es la que absorbe) ya tenia acceso a los commits de la rama que es absorvida.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Sí hay conflicto por que en ambos commits habia modificaciones en las mismas lineas del mismo archivo.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No hay conflicto. Hace un merge fast-forward.

**¿Qué comando o comandos utilizaste en el paso 25?**

git log --graph

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

En este caso en el que master absorve a title sí podria ser fast forwatd porque estan en linea. Pero lo han pedido no fast forward.

**¿Qué comando o comandos utilizaste en el paso 27?**

git reset HEAD~1 para volver al commit padre del commit segun la rama master. (Aunque tenga dos padres este comando hace que vuelva al commit anterior de la rama "original" por así decirlo, el commit anterior de la rama que ha absorvido a la otra, en este caso master.)

**¿Qué comando o comandos utilizaste en el paso 28?**

Para descartar cambios usamos git restore con el archivo del commit al que regresamos.

**¿Qué comando o comandos utilizaste en el paso 29?**

 git branch -D title

**¿Qué comando o comandos utilizaste en el paso 30?**

Primero usamos git reflog, buscamos el id del commit de cuando hemos hecho el merge y luego git reset y git restore.

**¿Qué comando o comandos usaste en el paso 32?**

Primero usamos git reflog para saber el id del commit inicial y luego git reset

**¿Qué comando o comandos usaste en el punto 33?**

Primero usamos git reflog para saber el id del commit al que ir y luego git reset
