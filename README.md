
# Examen git 

Adonay Gonzalez Gutierre


## Realiza la clonación del frepositorio creado.

**Comandos**

- git clone nombrerepositorio

*Salida*:

```code
dam@a108pc01:~/Documentos/ETS$ git clone git@github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
Clonando en 'ejercicio_git_adonay_gonzalez_gutierrez'...
warning: Pareces haber clonado un repositorio sin contenido.
dam@a108pc01:~/Documentos/ETS$ ls
2.txt  ejercicio_git_adonay_gonzalez_gutierrez  images  README.md  Unidad-1
dam@a108pc01:~/Documentos/ETS$ cd ejercicio_git_adonay_gonzalez_gutierrez/
```
## Añadir el archivo README al repositorio y realizar el primer commit.

**Comandos**

- touch nombre fichero
- git add .
- git commit -m"mensaje..."

*Salida:*

´´´code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ touch README.ddam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"primer commit"
[main (commit-raíz) 7fd7edf] primer commit
 1 file changed, 35 insertions(+)
 create mode 100644 README.md

´´´

## Crear una rama con nombre develop, Lista las ramas actuales.

**Comandos**:

- git branch develop
- git branch

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git branch develop
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git branch
  develop
* main

```
## Moverse a la rama y crear el fichero: hola.html. - Añadir el siguiente contenido: 

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Hola </title>
</head>
<body>
<h1 align="center" >Hola soy un título </h1>
<hr>
<p> Hola soy el alumno nombre_alumno </p>
</body>
</html>
```
**Comandos**:

- git checkout nombre de rama
- touch hola.html
- echo del contenido anterior

*Salida*
```code 
am@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git checkout develop
M	README.md
Cambiado a rama 'develop'
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ touch hola.html
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ nano hola.html

```