# EJERCICIO DE CLASE 2. Ejercicios básicos de MS-DOS 
### Hecho por Joan Pérez Susidko

## 1.- Crea la siguiente estructura de carpetas:
```
MD APLI PROG VARIOS
CD APLI
MD WORD ACCESS EXCEL
CD ..
CD PROG
MD BASIC PASCAL FROTRAN
CD ..
CD APLI/WORD
MD TEXTOS NOTAS
CD ..
CD EXCEL
MD TABLAS INFO
``` 
![image](https://user-images.githubusercontent.com/101748401/173261934-6e2543db-dab1-45d2-b8e2-3c4dbd20d17e.png)
![image](https://user-images.githubusercontent.com/101748401/173261940-911c8a59-8421-4ce9-8195-7e92ea5b36a7.png)

## 2.- Sitúate en la carpeta TABLAS
```
CD ./APLI/EXCEL/TABLAS/
```
![image](https://user-images.githubusercontent.com/101748401/173262087-11ceefa9-ea89-40a4-aa8e-b4b4e81d7126.png)

## 3.- Vuelve a la carpeta raíz
```
CD ../../
```
![image](https://user-images.githubusercontent.com/101748401/173262127-5b05ae17-9dbf-4912-bc2b-716782a2a0b9.png)
## 4.- Muestra el contenido de la carpeta PROG
```
DIR PROG
```
![image](https://user-images.githubusercontent.com/101748401/173262272-7d4dca9f-d1b0-465b-80ad-c174adfc1174.png)

## 5.- Borra la carpeta PASCAL
```
RD PASCAL
```
![image](https://user-images.githubusercontent.com/101748401/173262332-76198184-b1ea-4bea-92be-216539f5665d.png)

## 6.- Sitúate en la carpeta VARIOS y desde allí crea una nueva carpeta dentro de WORD llamado
```
CD VARIOS
MD PRACT
```
![image](https://user-images.githubusercontent.com/101748401/173262498-eecf28a7-fe8b-411e-bf7d-2a1074541243.png)

## 7.- Sitúate en PRACT y desde allí muestra el contenido de la carpeta EXCEL
```
CD ./APLI/WORD/PRACT/
DIR /HOME/JOAN/PRACTICAPOWERSHELL/APLI/EXCEL/
```

## 8.- Desde TABLAS muestra el listado de archivos y carpetas de la carpeta raíz
```
CD TABLAS
DIR /HOME/JOAN/PRACTICAPOWERSHELL
```
## 9.- Sitúate en la carpeta APLI y desde allí crea una subcarpeta llamada AGENDA dentro de VARIOS
```
CD APLI
MD /HOME/JOAN/PRACTICAPOWERSHELL/VARIOS/AGENDA
```
## 10.- Borra la carpeta EXCEL
```
RD /HOME/JOAN/POWERSHELL/APLI/EXCEL/
```
## 11.- Desde la carpeta raíz, crea en ella una subcarpeta llamada NUEVO
```
MD /HOME/JOAN/POWERSHELL/APLI/NUEVO
```
## 12.- Desde PRACT muestra el contenido de WORD
```
DIR /HOME/JOAN/POWERSHELL/APLI/WORD/
```
## EJERCICIO 2
## 1.- Utilizando el editor de textos de MS-DOS, crea un archivo de texto denominado EJER.TXT
```
copi con EJER.TXT
```
## 2.- Copia el archivo EJER.TXT en AGENDA
```
copi EJER.txt /home/JOAN/Practicapowershell/VARIOS/AGENDA/
```
## 3.- Borra el archivo almacenado en la carpeta TEXTOS
```
home/JOAN/Praticapowershell/APLI/WORD/TEXTOS> del EJER.TXT
```
## 4.- Añade el siguiente párrafo al archivo EJER.TXT:
```
echo “Cada archivo tiene un nombre y una extensión que los distingue del resto de archivos” > EJER.TXT
```
## 5.- Copia el archivo EJER.TXT en la carpeta BASIC
```
copy EJER.TXT /home/JOAN/Praticapowershell/PROG/BASIC
```
## 6.- Cambia el nombre del archivo almacenado en AGENDA por FICHERO.TXT
```
ren EJER.txt NUEVO.txt
dir
```
## 7.- Mueve el archivo FICHERO.TXT a la carpeta BASIC
```
move FICHERO.txt /home/JOAN/Practicapowershell/PROG/BASIC
```
## 8.- Abre el archivo EJER.TXT y borra la primera frase; almacena el nuevo archivo con el nombre NUEVO.TXT dentro de la carpeta BASIC
```
cd PROG/BASIC
notepad EJER.TXT
ren EJER.txt NUEVO.txt
```
## 9.- Copia el archivo NUEVO.TXT en la carpeta NOTAS
```
copy NUEVO.txt /home/JOAN/Practicapowershell/APLI/WORD/NOTAS
```
## 10.- ¿Cuántos archivos hay en la carpeta BASIC? ¿Y en NOTAS?
```
dir
dir /home/JOAN/Practicapowershell/APLI/WORD/NOTAS
```

## EJERCICIO 3

## 1.- Borra la carpeta ACCESS y en su lugar crea una nueva carpeta llamada ASTRO
```
del ACCESS
md ASTRO
```
## 2.- Crea la siguiente estructura de subcarpetas dentro de la carpeta ASTRO
```
cd ASTRO
md CIENCIA HISTORIA
cd CIENCIA
md ASTRO1 ASTRO3
cd ../
cd HISTORIA
md DATOS1 DATOS2
```
## 3.- Sitúate en la carpeta CIENCIA y desde allí muestra el listado de archivos y subcarpetas de la carpeta HISTORIA
```
cd CIENCIA
dir /home/JOAN/Practicapowershell/APLI/ASTRO/HISTORIA
```
## 4.- Utilizando el editor de MS-DOS crea el siguiente archivo de texto y guárdalo con el nombre TYCHO.TXT dentro de la carpeta DATOS1
```
cd DATOS
copy con TYCHO.txt
```
## 5.- Utilizando de nuevo el editor de textos de MS-DOS crea el siguiente archivo de texto, y guárdalo con el nombre KEPLER.TXT dentro de la carpeta DATOS2
```
cd DATOS2
copy con KEPLER.txt
```
## 6.- Copia los archivos TYCHO.TXT y KEPLER.TXT en la carpeta CIENCIA
```
copy KEPLER.txt /home/JOAN/Praticaspowershell/ASTRO/CIENCIA
cd ../
cd DATOS1
copy TYCHO.txt /home/JOAN/Praticaspowershell/ASTRO/CIENCIA
``` 
## 7.- Cambia de lugar los archivos almacenados en DATOS1 y DATOS2 de forma que TYCHO.TXT quede guardado dentro DATOS2 y KEPLER.TXT en DATOS1
```
move /home/JOAN/Praticaspowershell/DATOS2/HISTORIA
cd ../
cd DATOS2
move TYCHO.txt /home/JOAN/Praticaspowershell/APLI/ASTROS/HISTORIA/DATOS1/TYCHO.txt
```
## 8.- Crea un nuevo archivo formado por la unión de los dos anteriores (sin volver a escribir el texto) y guárdalo dentro de la carpeta HISTORIA con el nombre TOTAL.TXT
```
-copy *.txt KEPLER.txt
``` 
## 9.- Abre el archivo KEPLER.TXT almacenado en la carpeta CIENCIA y añade el siguiente texto:
```
cd CIENCIA
notepad KEPLER:TXT
```
## 10.- Cambia el nombre del archivo anterior por el de GALILEO.TXT
```
rename KEPLER.txt GALILEO.txt
``` 

## EJERCICIO 4

## 1.- Crea en la carpeta raíz de la unidad A: una carpeta denominada TECINFO
```
md TECINFO
```
## 2.- Crea dentro de TECINFO el siguiente archivo de texto y llámalo HARD.TXT
```
copy con HARD.txt
```
## 3.- Crea dentro de TECINFO el siguiente archivo de texto y llámalo SOFT.TXT
```
copy con SOFT.txt
```
## 4.- Mueve el contenido de TECINFO a la carpeta APLI del disquete A utilizado para realizar los ejercicios anteriores
```
move /home/JOAN/Practicapowershell/TECINFO/HARD.txt
move /home/JOAN/Practicapowershell/TECINFO/SOFT.txt
```
## 5.- Crea un nuevo archivo formado por la unión de HARD.TXT y SOFT.TXT, sin volver a escribir el texto, y guárdalo en la carpeta AGENDA con el nombre ORDER.TXT
```
copy *.txt ORDER.txt
```
## 6.- Elimina la carpeta TECINFO
```
del TECINFO
```
## 7.- Copia a la vez los archivos HARD.TXT y SOFT.TXT en la carpeta VARIOS
```
cd VARIOS
xcopy /home/JOAN/Practicapowershell/APLI
```
## 8.- Cambia la extensión de los archivos contenidos en AGENDA por .TYP
```
ren *.txt *.typ
```
