# Bienvenido a nuestro Repo de Git IA
## Ezequiel Lemos Cárdenas y Violeta Ai Naharro Zaldívar

## ¿Quién será el Alumno 1 y 2?
- Alumno 1 -> Ezequiel Lemos Cárdenas
- Alumno 2 -> Violeta Ai Naharro Zaldívar

## Alumno 1 
### Creación e inicialización de un repositorio 
- Añadimos al repositorio los archivos del documento Farmacia
```bash
git add .
git commit -m “Inicialización del repositorio con archivos Farmacia”
```
- Inicializamos el repositorio remoto creado en GitHub con nuestro repositorio local.
```bash
git remote add origin https://github.com/EzequielLemos/Practica-IA.git
```
- Revisamos que hemos agregado correctamente el repositorio remoto.
```bash
git remote
```
- Actualizamos el repositorio.
```bash
git push origin master
``` 
- ¿Qué ha ocurrido? ¿Se ha actualizado el repositorio?  

Salta un mensaje de error y no podemos actualizar el repositorio, pero con el siguiente comando ya funciona:

```bash
git push origin main
``` 
### Actualización README

Actualizamos el repositorio local con los cambios
```bash
git pull origin main
```
Posteriormente realizamos las modificaciones y volvemos a actualizar el repositorio  
```bash
git add README.md
git commit -m "Actualización del README con comandos hasta punto 5"
git push origin main
```
### Creación de ramas 

- Creamos la rama con

```bash
git branch ramaAlumno1
```
- Nos cambiamos a nuestra rama

```bash
git checkout ramaAlumno1
```
- Listamos las ramas con

```bash
git branch
```


## Alumno 2
Para clonar el repositorio, gracias a las extensiones de VSCode solo es necesario copiar el link del repositorio y pegarlo en la ventana de clonación.
Y ya que tengo extensiones de Git, puedo hacer un commit y un push directamente desde VSCode.
Ya creamos la rama con 
```bash

git branch raamaAlno2
```
Al darnos cuenta que el nombre de la rama estaba mal, la eliminamos con 
```bash
git branch -d raamaAlno2
```
Y creamos la rama con el nombre correcto
```bash
git branch ramaAlumno2
```
Y nos cambiamos a la rama con 
```bash
git checkout ramaAlumno2
```

## PREGUNTA 7
### En esta ocasión se pide listar el número de ramas que hay ahora mismo en tu proyecto. Cuando lo hayas hecho verás que hay un asterisco encima de una de las ramas del proyecto. ¿Qué significa?
En mi caso hay 2 ramas, la rama master y la ramaAlumno2. También se ven las ramas que existen en remoto, que se vería algo como
```bash
git branch -a
```

Usaríamos git branch -a para ver las ramas que existen tanto en remoto como en local. Lo que nos mostraría algo como:
```bash
  main
* ramaAlumno2
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/ramaAlumno2
```

El asterisco indica en qué rama estás trabajando en ese momento. Tras añadir mi compañero su rama esto se vería así:
```bash
  main
* ramaAlumno2
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/ramaAlumno1
  remotes/origin/ramaAlumno2
```


## PREGUNTA PUNTO 8
### En esta ocasión se pide listar el número de ramas que hay ahora mismo en tu proyecto. Cuando lo hayas hecho verás que hay un asterisco encima de una de las ramas del proyecto. ¿Qué significa?
```bash
git branch
```
El asterisco indica en qué rama estás trabajando en ese momento.

## PUNTO 9
Añadimos el archivo Cliente.java y lo subimos a la ramaAlumno2, según lo pone en el archivo de la práctica.

## PUNTO 10
### DIFERENCIAS ENTRE RAMAS
Para ver las diferencias entre las ramas, primero nos cambiamos a la rama master y posteriormente
```bash
git diff ramaAlumno1..ramaAlumno2
```
Con este comando mostramos las diferencias entre ambas ramas.  
Lo hemos logrado en menos de 2 minutos.

## Punto 11
### ¿habéis podido realizar los pasos de este ejercicio de forma idéntica? En caso negativo, explicar cuál creéis que el motivo por el que no habéis podido replicar los mismos comandos, con excepción de los nombres de las ramas personales.
Sí hemos podido aunque lo hemos hecho por separado, Violeta (alumno2) hizo su merge y luego Ezequiel (alumno1) hizo el suyo. Así no nos solapamos en ningún momento. Ezequiel hará los cambios pertinentes en el archivo Almacen_cli.java, Violeta hizo el merge y las modificaciones pertinentes del archivo README.md.

