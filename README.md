
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
- git push origin main (me equivoque al escribir los comandos e hice un push de todo )

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
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git branch
  develop
* main
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git merge develop
Ya está actualizado.
```
## Sube los cambios al repositorio a tu cuenta de Github.

**Comandos:**
 - git add .
 - git commit -m"mensaje"
 - git push

*salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git add .
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"subir cambios "
[main 71d1bbc] subir cambios
 1 file changed, 66 insertions(+), 2 deletions(-)
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push
Enumerando objetos: 5, listo.
Contando objetos: 100% (5/5), listo.
Compresión delta usando hasta 12 hilos
Comprimiendo objetos: 100% (3/3), listo.
Escribiendo objetos: 100% (3/3), 1.02 KiB | 1.02 MiB/s, listo.
Total 3 (delta 1), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
   2e99202..71d1bbc  main -> main

```

## Muestra todos los cambios realizados.
**Comados:**

- git diff

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git diff
diff --git a/README.md b/README.md
index ae155b3..0815be4 100644
--- a/README.md
+++ b/README.md
@@ -115,7 +115,7 @@ html
 **Comados:**
 - git add .
 - git commit -m"mensaje descriptivo"
-- git push
+- git push origin main (me equivoque al escribir los comandos e hice un push de todo )
 
 *Salida:*
 ```code
@@ -146,4 +146,70 @@ To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
 - git merge develop
 
 *Salida:*
+```code
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git branch
+  develop
+* main
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git merge develop
+Ya está actualizado.
+```
+## Sube los cambios al repositorio a tu cuenta de Github.
+
+**Comandos:**
+ - git add .
+ - git commit -m"mensaje"
+ - git push
+
+*salida:*
+```code
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git add .
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"subir cambios "
+[main 71d1bbc] subir cambios
+ 1 file changed, 66 insertions(+), 2 deletions(-)
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push
+Enumerando objetos: 5, listo.
+Contando objetos: 100% (5/5), listo.
+Compresión delta usando hasta 12 hilos
+Comprimiendo objetos: 100% (3/3), listo.
+Escribiendo objetos: 100% (3/3), 1.02 KiB | 1.02 MiB/s, listo.
+Total 3 (delta 1), reusados 0 (delta 0), pack-reusados 0
+remote: Resolving deltas: 100% (1/1), completed with 1 local object.
+To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
+   2e99202..71d1bbc  main -> main
+
+```
+
+## Muestra todos los cambios realizados.
+**Comados:**
 
+- git diff
+
+*Salida:*
+```code
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git diff
+diff --git a/README.md b/README.md
+index ae155b3..30d04d8 100644
+--- a/README.md
++++ b/README.md
+@@ -115,7 +115,7 @@ html
+ **Comados:**
+ - git add .
+ - git commit -m"mensaje descriptivo"
+-- git push
++- git push origin main (me equivoque al escribir los comandos e hice un push de todo )
+ 
+ *Salida:*
+ ```code
+@@ -146,4 +146,21 @@ To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
+ - git merge develop
+ 
+ *Salida:*
++```code
++dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git branch
++  develop
++* main
++dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git merge develop
++Ya está actualizado.
++```
+
+```
(END)


```
## Lista ahora los últimos cambios que se han producido en el repositorio, es decir, los últimos commits que han realizado en el repositorio.

**Comandos:**
- git log

*Salida*:
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git log
commit 71d1bbc60fc43cecf25de0e4984767ae768cd365 (HEAD -> main, origin/main)
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:25:31 2023 +0100

    subir cambios

commit 2e99202ad409524009c600f86ab3a7970c024309
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:17:33 2023 +0100

    mensaje descriptivo

commit 7fd7edf071803d364557b15eb2ee713595f49e7a (develop)
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 14:58:38 2023 +0100

    primer commit

```

## Lista todos los tags(etiquetas que existan) Crea una nueva etiqueta (tag) de nombre v.1 y sube los cambios.
**Comandos:**
- git tag
- git tag v.1

*Salida*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git tag
ls
v.1
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git tag v.1
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git add .
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"seguimos trabajando"
[main 20d6896] seguimos trabajando
 1 file changed, 158 insertions(+), 1 deletion(-)
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push
Enumerando objetos: 5, listo.
Contando objetos: 100% (5/5), listo.
Compresión delta usando hasta 12 hilos
Comprimiendo objetos: 100% (3/3), listo.
Escribiendo objetos: 100% (3/3), 2.37 KiB | 2.37 MiB/s, listo.
Total 3 (delta 0), reusados 0 (delta 0), pack-reusados 0
To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
   71d1bbc..20d6896  main -> main

```
hice los pasos al reves primero la cree y luego las liste

## Crea la feature-2 y muevete a esta.
 **Comandos**:
 - git branch feature-2
 - git checkout feature-2

*Salida:*
```code
am@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git branch feature-2
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git checkout feature-2
M	README.md
Cambiado a rama 'feature-2'
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ touch  Estamos_a_punto_de_terminar.html
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ nano  Estamos_a_punto_de_terminar.html
  GNU nano 6.2            Estamos_a_punto_de_terminar.html                      
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/s>
<html>
<head>
<title>Terminando </title>
</head>
<body>
<h1 align="center" >Apunto de terminar </h1>
<hr>
<p> Esto se esta acabando Adonay </p>
</body>
</html>

```
## Realiza el commit y sube los cambios.
**Comandos:**
- git add .
- git commit -m

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git add .
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"nueva rama"
[feature-2 e30c108] nueva rama
 2 files changed, 67 insertions(+), 1 deletion(-)
 create mode 100644 Estamos_a_punto_de_terminar.html

```
## Muevete a la rama develop, y realiza la mezcla con la rama feature-2.

**Comandos:**
- git checkout develop
- git merge feature-2

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git checkout develop
Cambiado a rama 'develop'
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git merge feature-2
Actualizando 7fd7edf..7c56476
Fast-forward
 Estamos_a_punto_de_terminar.html |  11 ++
 README.md                        | 341 ++++++++++++++++++++++++++++++++++++++-
 adios.html                       |  13 ++
 hola.html                        |  13 ++
 4 files changed, 377 insertions(+), 1 deletion(-)
 create mode 100644 Estamos_a_punto_de_terminar.html
 create mode 100644 adios.html
 create mode 100644 hola.html

```

## sube los cambios de la rama develop a Github.

**Comandos:**

- git add .
- git commit -m ""
- git push --set-upstream origin develop

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push --set-upstream origin develop
Enumerando objetos: 5, listo.
Contando objetos: 100% (5/5), listo.
Compresión delta usando hasta 12 hilos
Comprimiendo objetos: 100% (3/3), listo.
Escribiendo objetos: 100% (3/3), 559 bytes | 559.00 KiB/s, listo.
Total 3 (delta 2), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'develop' on GitHub by visiting:
remote:      https://github.com/adogonz23/ejercicio_git_adonay_gonzalez_gutierrez/pull/new/develop
remote: 
To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
 * [new branch]      develop -> develop
Rama 'develop' configurada para hacer seguimiento a la rama remota 'develop' de 'origin'.

```
## Cambia a la rama principal, realiza la mezcla con la rama develop.

**Comandos**
- git chekout main
- git merge develop

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git checkout main
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git merge develop
Actualizando 20d6896..57a14e4
Fast-forward
 Estamos_a_punto_de_terminar.html |  11 ++++
 README.md                        | 131 ++++++++++++++++++++++++++++++++++++++-
 2 files changed, 141 insertions(+), 1 deletion(-)
 create mode 100644 Estamos_a_punto_de_terminar.html

```
## Realiza el tag con el nombre v.2. y sube los cambios.

**Comandos:**
- git tag v.2
- git add .
- git commit -m"tag v.2"
- git push

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git tag v.2
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"a"
[main c06ad16] a
 1 file changed, 18 insertions(+), 1 deletion(-)
am@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push
Enumerando objetos: 5, listo.
Contando objetos: 100% (5/5), listo.
Compresión delta usando hasta 12 hilos
Comprimiendo objetos: 100% (3/3), listo.
Escribiendo objetos: 100% (3/3), 515 bytes | 515.00 KiB/s, listo.
Total 3 (delta 2), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
   20d6896..c06ad16  main -> main

```
## Muestra todos los cambios realizados en el repositorio. Muestra todos los commits realizados

**Comandos:**
- git diff 
- git log

*Salida:*
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git log
commit c06ad16c2e96940344c25ca86bee2dc13001a29b (HEAD -> main, origin/main)
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:57:53 2023 +0100

    a

commit 57a14e4340026143e84e2465cd63fbb99886db24 (tag: v.2, origin/develop, develop)
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:54:04 2023 +0100

    a

commit c1b8e25e78a682f2017f85c18f4da10a0dbcce64
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:49:56 2023 +0100

    subimos a rama develop

commit 7c56476714ce6047eb35810d76ad7525565b1730 (origin/feature-2, feature-2)
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:46:18 2023 +0100

    a

commit e30c108c6bdffa8729834772b2c8053e27086070
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:43:18 2023 +0100

    nueva rama

commit 20d68967e07b00e5d7e37ffe08a39a4fd7ff81a2
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:38:16 2023 +0100

    seguimos trabajando

commit 71d1bbc60fc43cecf25de0e4984767ae768cd365 (tag: v.1, tag: ls)
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:25:31 2023 +0100

    subir cambios

commit 2e99202ad409524009c600f86ab3a7970c024309
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 15:17:33 2023 +0100

    mensaje descriptivo

commit 7fd7edf071803d364557b15eb2ee713595f49e7a
Author: adogonz23 <adogonzalez75@gmail.com>
Date:   Wed Oct 18 14:58:38 2023 +0100

    primer commit
(END)


```
```code
dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git diff
diff --git a/README.md b/README.md
index cf309e7..a43be9b 100644
--- a/README.md
+++ b/README.md
@@ -450,3 +450,91 @@ Fast-forward
 - git add .
 - git commit -m"tag v.2"
 - git push
+
+*Salida:*
+```code
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git tag v.2
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git commit -m"a"
+[main c06ad16] a
+ 1 file changed, 18 insertions(+), 1 deletion(-)
+am@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git push
+Enumerando objetos: 5, listo.
+Contando objetos: 100% (5/5), listo.
+Compresión delta usando hasta 12 hilos
+Comprimiendo objetos: 100% (3/3), listo.
+Escribiendo objetos: 100% (3/3), 515 bytes | 515.00 KiB/s, listo.
+Total 3 (delta 2), reusados 0 (delta 0), pack-reusados 0
+remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
+To github.com:adogonz23/ejercicio_git_adonay_gonzalez_gutierrez.git
+   20d6896..c06ad16  main -> main
+
+```
+## Muestra todos los cambios realizados en el repositorio. Muestra todos los commits realizados
+
+**Comandos:**
+- git diff 
+- git log
+
+*Salida:*
+```code
+dam@a108pc01:~/Documentos/ETS/ejercicio_git_adonay_gonzalez_gutierrez$ git log
+commit c06ad16c2e96940344c25ca86bee2dc13001a29b (HEAD -> main, origin/main)
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:57:53 2023 +0100
+
+    a
+
+commit 57a14e4340026143e84e2465cd63fbb99886db24 (tag: v.2, origin/develop, develop)
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:54:04 2023 +0100
+
+    a
+
+commit c1b8e25e78a682f2017f85c18f4da10a0dbcce64
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:49:56 2023 +0100
+
+    subimos a rama develop
+
+commit 7c56476714ce6047eb35810d76ad7525565b1730 (origin/feature-2, feature-2)
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:46:18 2023 +0100
+
+    a
+
+commit e30c108c6bdffa8729834772b2c8053e27086070
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:43:18 2023 +0100
+
+    nueva rama
+
+commit 20d68967e07b00e5d7e37ffe08a39a4fd7ff81a2
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:38:16 2023 +0100
+
+    seguimos trabajando
+
+commit 71d1bbc60fc43cecf25de0e4984767ae768cd365 (tag: v.1, tag: ls)
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:25:31 2023 +0100
+
+    subir cambios
+
+commit 2e99202ad409524009c600f86ab3a7970c024309
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 15:17:33 2023 +0100
+
+    mensaje descriptivo
+
+commit 7fd7edf071803d364557b15eb2ee713595f49e7a
+Author: adogonz23 <adogonzalez75@gmail.com>
+Date:   Wed Oct 18 14:58:38 2023 +0100
+
+    primer commit
+(END)
+
+
+```
+```code
+
+```
\ No newline at end of file
(END)

```