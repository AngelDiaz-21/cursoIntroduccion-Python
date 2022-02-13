# Módulo 2 - Crear y administrar proyecto (Katas)

## Ejercicio - Crear un paquete

Utilizar un entorno virtual como una forma para afectar a los paquetes instalados globalmente u otros.

### Crear un entorno virtual

Desde la terminal accederemos al directorio donde se guardara el proyecto.

![Directorio del proyecto](/Images/directorio-Proyecto.png "Directorio donde se encuentra el proyecto")

Se creará un entorno virtual mediante *venv*. Se ejecutará el siguiente comando:
`python -m venv env`
Después, ejecutaremos el siguiente comando para activar el entorno virtual:
`env\Scripts\activate`

![Creación del entorno virtual](/Images/creacion-entornoVirtual.png "Creación del entorno virtual")

### Instalar una biblioteca

Para ver las bibliotecas instaladas en el entorno ejecutaremos el siguiente comando:
`pip freeze`

Sin embargo, no hay respuesta, así que a continuación se instalará la biblioteca *dateutil* (paquete para analizar el formato de archivo *.yml*), con el siguiente comando:
`pip install python-dateutil`

Dando como resultado un mensaje que la bilioteca se ha instalado.

![Instalación de la biblioteca](/Images/instalar-biblioteca.png "Instalación de la biblioteca")

**Nota:**
Para solucionar el warning que nos sugiere actualizar la versión de pip de 21.2.4 a la versión 22.0.3 tenemos que ir al directorio que nos menciona y ejecutar el comando:
`python -m pip install --upgrade pip`

Volveremo a ejecutar el comando *pip freeze* para ver la lista de bibliotecas.

![Lista de bibliotecas instaladas](/Images/bibliotecas-instaladas.png "Lista de bibliotecas instaladas")

### Desactivar un entorno virtual

Cuando se esta trabajando en varios proyectos de Python y se necesite cambiar entre se debe salir (desactivar) el entorno virtual. Para eso se ejecuta el siguiente comando:
`deactivate`

![Desactivar el entorno virtual](/Images/deactivate-entornoVirtual.png "Desactivar el entorno virtual")
