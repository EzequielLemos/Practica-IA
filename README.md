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


## PREGUNTA PUNTO 10

Llega el jefe de tu equipo al despacho en 2 minutos, solo ha venido para ver las diferencias entre los dos códigos antes de subirlo al repositorio común. Así que busca rápido cómo ver las diferencias entre ramas. 

```bash
git diff ramaAlumno1..ramaAlumno2
```
Con este comando mostramos las diferencias entre ambas ramas.  
Lo hemos logrado en menos de 2 minutos.
