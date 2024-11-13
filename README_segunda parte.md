## PUNTO 14
### Unión de dos nuevos alumnos
Nuestro equipo (Ezequiel y Violeta) se ha unido al GitHub de Marta y Pablo. Quedando una estructura tal que:
Alumno 1 -> Marta Jones González
Alumno 2 -> Pablo del Valle Davoodzadeh
Alumno 3 -> Ezequiel Lemos Cárdenas
Alumno 4 -> Violeta Ai Naharro Zaldívar

## PUNTO 15
### Crear ramas remotas (Alumno 3 y 4) y una extra para investigar (Alumno 1 y 2)
Creamos la rama de forma remota con 
```bash
git branch ramaAlumno4
git push --set-upstream origin ramaAlumno4
``` 

El último comando lo que hace es crear la rama remota y que aparezcan a nivel remoto.
## PUNTO 16

## PUNTO 17
Busca en la ayuda de este comando para visualizar los últimos cambios realizados de tal modo que aparezca
la siguiente información:
▪ sha1
▪ autor
▪ quién hizo el commit
▪ mensaje del commit

Hemos mirado la doumentación y foros varios y hemos visto que el comando git whatchanged ha quedado obsoleto y que se recomienda usar git log con el siguiente formato para que se consiga la información requerida:
```bash
git log --pretty=format:"%h %an %ae %s"
```