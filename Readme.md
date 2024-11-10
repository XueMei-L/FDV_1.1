# FDV_1.1 


```
>>  PRACTICA:   Unity Project 1.1 - Herramienta Git LFS
>>  COMPONENTE: XueMei Lin
>>  GITHUB:     https://github.com/XueMei-L/FDV_1.1.git
```

# Proceso de la practica 1.1
### Paso1. Crear una carpeta que incluye 2 imagenes y 3 ficheros
Lista de imagenes y ficheros:
**1. *VanGogh.jpg*
2. *VanGogh2.jpg*
3. *file1.txt*
4. *file2.txt*
5. *file3.txt***


### Paso2. Crear repositorio FDV_1.1
Se crea el repositorio en github llamado **FDV_1.1**

![Project Screenshot](img/img1.png)

### 3. Realizar Git y subir al repositorio
Se sube los ficheros iniciales al repositorio con los siguientes comandos:

1. Usa el comando **`git init`** para inicializar el repositorio de Git.
2. Agrega todos los archivos al área de preparación usando **`git add .`**.
3. Ejecuta el siguiente comando para realizar el primer commit:
   **`git commit -m "Initial commit with images and text files"`**
4. Cambia el nombre de la rama principal a main **`git branch -m main`**
5. Añade el repositorio remoto en GitHub: **`git remote add origin https://github.com/XueMei-L/FDV_1.1.git`**
6. Empuja los cambios al repositorio remoto en GitHub usando:
   **`git push -u origin main`**

### Paso3. Instalar GIt LFS y subir los cambios al repositorio
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
