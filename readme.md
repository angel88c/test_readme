  

# iBScrypter Guía de inicio rápido

Esta guía está hecha con el propósito de crear el entorno necesario para empezar a desarrollar script de python y ejecutarlos mediante la herramienta iBScrypter.

<div>
    <img src="./images/iBScrypter.Net.png" width="800"> 
<div>

## Prerequisitos

El proyecto trabaja solamente con windows 10/11, para previas versiones de windows no se ha probado.

  

*  <img src="./images/CS.svg" width="20"> Net 6 runtime version 6.0.9
*  <img src="./images/Python-Dark.svg" width="25"> Python version 3.9.13
*  <img src="./images/iBscrypter.png" width="20"> iBscrypter
*  <img src="./images/win10.png" width="20"> Windows 10/11
  

## Instalación

1. Descargue e instale la version de .Net 6 Desktop runtime, la versión recomendada es la 6.0.9 de la página oficial de microsoft; seleccione .Net 6 Desktop runtime 6.0.9 dependiendo de su arquitectura de windows x86 o x64 https://dotnet.microsoft.com/en-us/download/dotnet/6.0 Descargue de la página oficial de Microsoft o de la carpeta descargada en el punto 3.

    <img src="./images/.net1.png">
    <br><br>
    <img src="./images/.net2.png">

2. Descargue e instale python para windows, la versión recomendada para desarrollar sus programas para el iBScrypter es la versión 3.9.13, descargue de la página oficial de python o de la carpeta descargada en el punto 3.

    https://www.python.org/downloads/release/python-3913/

    Seleccione el instalador marcado como recomendado de acuerdo a sus sitema operativo y arquitectura.

    <img src="./images/python1.png">
  

3. Descargue e instale iBScrypter con el instalador proporcionado por iBtest de la fuente **installer win-x64/setup.exe** [**iBScrypter_v1.0**](https://drive.google.com/file/d/1t2hSy8Deab49Yz0OU6weX69jKZVjlR8p/view?usp=sharing)

4. Descomprima el archivo *.zip y copie la carpeta script_example de la carpeta descargada y peguela de preferencia en **C:\iBtest\iBScrypter scripts\\** ya que esta es la ruta que tiene definido el archivo de configuración **iBScrypter_ConfigX.ini** por defecto.

5. Verifique la ruta de instalación del interprete de python, abriendo una ventana de comandos (cmd) y ejecutando el siguiente comando



```bash
where python
```

output ejemplo:

  

```bash
C:\Users\c_ang\AppData\Local\Programs\Python\Python39\python.exe
C:\Users\c_ang\AppData\Local\Microsoft\WindowsApps\python.exe
```

  
  

Si tiene más de una versión de python instalada, seleccione la que corresponda a la versión 3.9. copie la ruta obtenida y peguela en el archivo **iBScrypter_configX.ini** en la sección **[PythonEnvironment]** en el valor de la llave **PythonInterpreter**.

```bash
[PythonEnvironment]
PythonInterpreter = "C:/Users/c_ang/AppData/Local/Programs/Python/Python39/python.exe"
```  

Asegúrese de que la ruta esté entre comillas dobles para evitar errores cuando la ruta tenga espacios en blanco.

1. Vaya a la carpeta script_example y copie la ruta completa del archivo de ejemplo template_script.py, péguelo en la ruta correspondiente a STD en el archivo de configuración **iBScrypter_ConfigX.ini**

7. Ejecute el programa iBScrypter.exe y siga los siguientes pasos:

- Haga click en el botón Load Script y seleccione el script STD.\
    <br><br>
    <img src="./images/ib1.png">
    <br><br>
    Si todo está correcto con el script, el log registrará el siguiente mensaje indicando que el archivo no tiene errores de sintaxis.

    ```text
    [11.19.2022 17:21:01.467] Script was Loaded. without syntax errors.
    ```
  
- Haga click en el botón Start para arrancar la ejecución del script. \
    <br><br>
    <img src="./images/ib2.png">
    <br><br>
    Si todo está correcto debería terminar la ejecución y establecer un estatus random de la ejecución, Pass or Fail.
 


Con esto ya podrá desarrollar sus propios programas de script en python para sus estaciones de automatización.