
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
- nano hola.html escribir el codigo anterior

*Salida*
```code 
am@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git checkout develop
M	README.md
Cambiado a rama 'develop'
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ touch hola.html
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ nano hola.html

```

## Moverse a la rama principal y crear el fichero adios.html > Sustituye nombre_alumno por tu nombre.

**Comandos**

- git checkout main
- touch adios.html
- nano adios.html (escribri el codigo y sustituir el nombre)

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ touch adios.html
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ nano adios.html
 GNU nano 6.2                             adios.html                                       
html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Adios </title>
</head>
<body>
<h1 align="center" >Adios soy un título </h1>
<hr>
<p> Adios soy el alumno Adonay </p>
</body>
</html>
```
## Crea el commit con un mensaje descriptivo, sube los cambios a la rama actual.

**Comados:**
- git add .
- git commit -m"mensaje descriptivo"
- git push

*Salida:*
```code
am@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git add .
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"mensaje descriptivo"
[main 2e99202] mensaje descriptivo
 3 files changed, 77 insertions(+), 1 deletion(-)
 create mode 100644 adios.html
 create mode 100644 hola.html
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push
Enumerando objetos: 8, listo.
Contando objetos: 100% (8/8), listo.
Compresión delta usando hasta 12 hilos
Comprimiendo objetos: 100% (7/7), listo.
Escribiendo objetos: 100% (8/8), 1.58 KiB | 807.00 KiB/s, listo.
Total 8 (delta 2), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (2/2), done.
To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
 * [new branch]      main -> main

```

## Lista las ramas actuales ,Realizar la mezcla en el repositorio principal.

**Comando:**

- git branch
- git merge develop

*Salida:*

