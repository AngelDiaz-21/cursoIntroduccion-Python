# Uso de tracebacks para buscar errores

## Tracebacks

Si intentamos en un notebook, abrir un archivo inexistente sucede lo siguiente:

![Abrir archivo inexistente](../images/archivoInexistente_notebook.png "Abrir archivo inexistente")

Intenta crear un archivo de Python y asígnale el nombre open.py, con el contenido siguiente:

![Contenido en el archivo open.py](../images/contenido_Open_py.png "Contenido en el archivo open.py")

Ejecútala con Python y podrás comprobar el siguiente mensaje de error:

![Mensaje de error en open.py](../images/mensajeError_Open_py.png "Mensaje de error en open.py")

## Controlando las excepciones

### Try y Except de los bloques

Vamos a usar el ejemplo de navegador a fin de crear código que abra archivos de configuración para la misión de Marte. Los archivos de configuración pueden tener todo tipo de problemas, por lo que es fundamental notificarlos con precisión cuando se presenten. Sabemos que, si no existe un archivo o directorio, se genera FileNotFoundError. Si queremos controlar esa excepción, podemos hacerlo con un bloque try y except:

![Controlar excepción si no existe un archivo](../images/archivoInexistente_txt.png "Controlar excepción si no existe un archivo")

Vamos a crear un archivo de Python denominado config.py. El archivo tiene código que busca y lee el archivo de configuración del sistema de navegación:

![Archivo config.py ](../images/archivo_config.png "Código para buscar y leer el archivo de configuración")

Probaremos actualizando la función main(). Ahora volvemos a ejecutar el código en el mismo lugar donde existe el archivo config.txt con permisos incorrectos:

![Actualización funcion main() ](../images/actualizar_Main.png "Actualización de la función main() y mostrando el error")

Vamos a corregir este fragmento de código para abordar todas estas frustraciones. Revertiremos la detección de FileNotFoundError y luego agregamos otro bloque except para detectar PermissionError: