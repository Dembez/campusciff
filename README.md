# campusciff

# Ejercicio práctico sobre la utilización básica de Git, GitHub y Markdown

### Crear un repositorio en vuestro GitHub llamado campusciff

![Creative	Commons	BY	SA](C:\Users\66880816\Desktop\GitHub\1.png)

### Clonar vuestro repositio en local.

git clone git@github.com:Dembez/campusciff.git

###  Añadir al README.md los comandos utilizados hasta ahora y hacer un commit inicial con el mensaje commit inicial

cd campusciff

git commit -m "añadidos comandos a Readme.md"

### Subir los cambios al repositorio remoto

git push origin master

### Crear en el repositorio local un fichero llamado privado.txt

echo "privado" > privado.txt

###  Crear en el repositorio local una carpeta llamada privada

mkdir privada

###  Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.

echo "privado.txt" > .gitignore

cat .gitignore

privada/

git add .gitignore

git commit -m "añadido .gitignore"

### Añadir fichero 1.txt al repositorio local. 

echo "" > 1.txt

git add -A

git commit -m "añadido 1.txt" 

### Crear un tag v0.1

git tag v0.1

git add -A

git commit -m "añadido tag v0.1"

### Subir los cambios al repositorio remoto

git push origin master

### Poner una foto en vuestro perfil de GitHub. 

![](C:\Users\66880816\Desktop\GitHub\2.png)

### Poner el doble factor de autentificación en vuestra cuenta de GitHub

![](C:\Users\66880816\Desktop\GitHub\3.png)

### Añadir (si no lo habéis hecho ya) la clave pública que se corresponde a tu ordenador

$ ssh-keygen -t rsa -b 4096 -C "borjamendez@campusciff.net"

clip < ~/.ssh/id_rsa.pub

GitHub --> SSH and GPG keys --> New SSH key

ssh -T git@github.com

### Preguntar los nombres de usuario de GitHub de tus compañeros de clase, búscalos, y sigueles. Seguir los repositorios campusciff del resto de tus compañeros. Añadir una estrella a los repositorios campusciff del resto de tus compañeros.

![](C:\Users\66880816\Desktop\GitHub\4.png)

### Crear una tabla de este estilo en el fichero README.md con la información de varios de tus compañeros de clase:

| NOMBRE            | GITHUB                                            |
| ----------------- | -----------------------------------------------:  |
| Alberto Marino    | [Alberto Marino](https://github.com/amarino5)     |
| Enrique Serrano   | [Enrique Serrano](https://github.com/eserranom)   |
| Araceli Macía     | [Araceli Macía](https://github.com/araceliMacia)  |
| Giovani Mata      | [Giovani Mata](https://github.com/giovamata)      |
| Ainhoa Calvo      | [Ainhoa Calvo](https://github.com/AinhoaCE)       |
| Mark Wellings     | [Mark Wellings](https://github.com/Mark-Wellings) |
| Fernando Escolano | [Fernando Escolano](https://github.com/fescolan)  |
| Anna Lawrence     | [Anna Lawrence](https://github.com/annalawrenc)   |
| Juan García	    | [Juan García](https://github.com/juangarciaciff)  |
| Asier Matas       | [Asier Matas](https://github.com/asiermatas)      |


### Poner a github.com/asanzdiego como colaborador del repositorio campusciff

![](C:\Users\66880816\Desktop\GitHub\5.png)


# Ejercicio práctico sobre la utilización avanzada de Git, GitHub y Markdown 

### Crear una rama v0.2. 

git branch v0.2

### Posiciona tu carpeta de trabajo en esta rama

git checkout v0.2

### Añadir un fichero 2.txt en la rama v0.2. 

echo "" > 2.txt

git add -A

git commit -m 'añadir fichero 2.txt en la rama v0.2'

### Subir los cambios al reposiorio remoto

git push origin v0.2

### Posicionarse en la rama master

git checkout master

### Hacer un merge de la rama v0.2 en la rama master

git merge origin v0.2

### En la rama master poner Hola en el fichero 1.txt y hacer commit

echo "Hola" >> 1.txt git add -A git commit -m "poner Hola en el fichero 1.txt"

### Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit

git checkout v0.2

echo "Adios" >> 1.txt

git add -A

git commit -m "poner Adios al fichero 1.txt"

### Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2

git checkout master

git merge v0.2

### Listar las ramas con merge y las ramas sin merge.

git	branch	--merged

git	branch	--no-merged

### Arreglar el conflicto anterior y hacer un commit

Borrar sobrante en fichero

git add -A

git commit -m "Arreglar conflicto en fichero 1.txt" 1.txt

### Crear un tag v0.2 

git tag -a v0.2 -m "Añadir Adios en fichero 1.txt" b2f06b6

### Borrar la rama v0.2

git branch -d v0.2

###  Listar los distintos commits con sus ramas y sus tags

git list

### Crear una organización llamada campusciff-tunombredeusuariodegithub 

![](C:\Users\66880816\Desktop\GitHub\6.png)

### Crear 2 equipos en la organización campusciff-tunombredeusuariodegithub, uno llamado administradores con más permisos y otro colaboradores con menos permisos. 


