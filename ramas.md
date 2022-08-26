# Gestionando ramas
Comandos útiles de git para la gestión de ramas en modo local y remoto


## Creando ramas
Sintaxis general: 

	git branch <nombre-de-la-nueva-rama>

Ejemplo: 

	git branch rama1


## Desplazándose entre ramas
Podemos movernos entre las diferentes ramas exixtentes. 

Sintaxis general: 

	git checkout <nombre-de-la-rama>

Ejemplo: 

	git checkout rama1

Y obtendremos una salida similar a esta: 


```bash
  main
* rama1
```


## Fusionando ramas
Procedimiento destinado a combinar el contenido de una rama en la rama actual.

Sintaxis general: 

	git merge <nombre-de-la-rama-a-fusionar-con-la-rama-actual>

Ejemplo: 

	git merge rama1

El comando anterior fusionará el contenido de la rama `rama1` con el contenido de la rama actual. 


## Cargando la rama local en remoto
Para tener una copia de la rama local en remoto (uptstream), la sintaxis general es: 

	git push --set-upstream origin <nombre-de-la-rama-local>

Por ejemplo:

	git push --set-upstream origin rama1

El comando anterior creará la `rama1` de manera remota. 


## Borrando ramas
Al borrar una rama, borraremos también su contenido. Borrar una rama local no implica borrar su copia remota, y viceversa. 

### Eliminando una rama local
Sintaxis general: 

	git branch -d <nombre-de-la-rama-a-eliminar>


Ejemplo: 

	git branch -d rama1

El comando anterior eliminará la rama local  `rama1`  y su contenido.

### Eliminando una rama remota
Sintaxis general: 

	git branch -d <nombre-de-la-rama-a-eliminar>


Ejemplo: 

	git branch -d rama1

El comando anterior eliminará la rama local  `rama1`  y su contenido.

NOTA: No es posible eliminar la rama actual. En otras palabras, para eliminar una rama determinada tendremos que estar ubicados en una rama distinta a la que deseamos eliminar. 



