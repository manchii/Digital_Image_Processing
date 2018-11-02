# Transformaciones Geométricas


#### Descripción de la Aplicación

La aplicación implementada utiliza una clase que sigue el patrón de
diseño denominado **funtor**, para aplicar transformaciones geométricas de imágenes.

La descripción del patrón de diseño **funtor** se puede encontrar en la página de ***Arquitectura*** en la documentación oficial de la biblioteca LTI-Lib2:
http://www.ie.tec.ac.cr/palvarado/ltilib-2/html/architecture.html

La aplicación aplica el siguiente mapeo bilineal por defecto: 
$$\text{w}=\frac{az+b}{cz+d}$$

Donde:
$$a=2.1+2.1j$$
$$b=0$$
$$c=0,003$$
$$d=1+j$$

### Prerequisitos

La máquina donde se desea ejecutar la aplicación debe contar con: 
* Sistema Operativo Linux
* Biblioteca LTI-Lib-2

### Instrucciones de Uso

##### Compilación
En el repositorio se presenta un archivo denominado *Makefile* junto a los demás archivos de código fuente. Basta con abrir una terminal desde la carpeta del repositorio y ejecutar:
```
make
```
##### Ejecución
Si la compilación finalizó correctamente se generará un archivo ejecutable denominado *Tarea_04*. 

###### * Imagen a Utilizar: 
El *path* de la imagen a utilizar debe colocarse después del nombre del ejecutable de acuerdo a la versión del programa:
```
./Tarea_04 <path_imagen>
```

###### * Resultado de Ejemplo:
Con los parámetros del mapeo por defecto se obtiene el siguiente resultado:

![](lennaResult.png)

Los parámetros de dicho mapeo se pueden modificar en el archivo denominado **bilinear.dat**
