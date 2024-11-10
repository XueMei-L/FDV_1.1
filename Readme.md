# FDV_1.1 


```
>>  PRACTICA:   Unity Project 1.1 - Herramienta Git LFS
>>  COMPONENTE: XueMei Lin
>>  GITHUB:     https://github.com/XueMei-L/FDV_1.1.git
```

# Proceso de la practica 1.1
### Paso1. Crear una carpeta que incluye 2 imagenes y 3 ficheros
Lista de imagenes y ficheros:
***1. VanGogh.jpg
2. VanGogh2.jpg
3. file1.txt
4. file2.txt
5. file3.tx**t*


### Paso2. Crear repositorio FDV_1.1
Se crea el repositorio en github llamado **FDV_1.1**

![Project Screenshot](img/image0.png)

### Paso3. Realizar Git y subir al repositorio
Se sube los ficheros iniciales al repositorio con los siguientes comandos:

1. Usa el comando **`git init`** para inicializar el repositorio de Git.
2. Agrega todos los archivos al área de preparación usando **`git add .`**.
3. Ejecuta el siguiente comando para realizar el primer commit:
   **`git commit -m "Initial commit with images and text files"`**
4. Cambia el nombre de la rama principal a main **`git branch -m main`**
5. Añade el repositorio remoto en GitHub: **`git remote add origin https://github.com/XueMei-L/FDV_1.1.git`**
6. Empuja los cambios al repositorio remoto en GitHub usando:
   **`git push -u origin main`**

### Paso4. Instalar GIt LFS y subir los cambios al repositorio
1. Instala Git LFS (Large File Storage) en el repositorio local:
   ```bash
   git lfs install
2. Configura Git LFS para hacer seguimiento de archivos de imagen .jpg y .png:
    ```bash
   git lfs track "*.png" "*.jpg"
Esto crea un archivo .gitattributes en el repositorio, que indica a Git LFS que maneje archivos .jpg y .png como archivos grandes.

3. Tras de realizar los cambios, hace una captura del seguimiento de LFS y añadir un fichero adicional.
   1. ***seguimientoLFS.png***
   2. ***file4.txt***
   

4. Actualizamos el repositorio
```
   git add .
   git commit -m "lsf process"
   git push
```

### Paso5. Crear repositorio para la practica 1.2
Se crea otro repositorio en Github llamado **FDV1.2**
![alt text](img/image1.png)

### Paso6. Realizar git LFS en el FDV.1.2
1. Agrega un **script1.2.cs** y una textura **textura.txt**

**script1.2.cs: **
```
using UnityEngine;

public class ScriptTarea1_2 : MonoBehaviour
{
    void Start()
    {
        Debug.Log("Script tarea 1.2");

    }
}
```

2. realiza los siguientes comandos con git LFS:

Instalar Git LFS y añadir tipos de ficheros que deseamos.
```
git lfs install
```
```
git lfs track "*.png" "*.jpg" "*.tif" "*.tga"
```
```
git lfs track "Script1_2.cs"
```
![alt text](img/image2.png)