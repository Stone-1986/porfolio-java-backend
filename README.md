## _Configuración de un repositorio_
Cómo configurar un repositorio con el sistema de control de versiones Git, se explicará cómo iniciar un repositorio de Git para un proyecto nuevo o existente.

## _Qué es un repositorio de Git_
Sirve básicamente para gestionar las versiones por las que va pasando el código de los proyectos y a las que se puede acceder cuando lo necesites.Físicamente no es más que una carpeta del sistema de archivos con código fuente de una aplicación. Esa carpeta se mantiene bajo el seguimiento de Git, de modo que, si se realizan cambios en sus archivos, se mantienen controlados por el sistema.
Git tiene la característica de ser un sistema de control de versiones con repositorios distribuidos. Esto quiere decir que cada uno de los integrantes de un proyecto tiene una copia exacta del repositorio y no solamente una copia de los archivos con los que haya trabajado.

## _Inicio de un nuevo repositorio: git init_
El comando git init crea un nuevo repositorio de Git. Puede utilizarse para convertir un proyecto existente y sin versión en un repositorio de Git, o para inicializar un nuevo repositorio vacío.

### _ejemplo_
Primero se debera establecer el directorio de la carpeta raíz del proyecto con el comando cd y luego ejecutar git init.
```
  cd /path/to/your/existing/code 
  git init
```

## _Clonación de un repositorio existente: git clone_
  
