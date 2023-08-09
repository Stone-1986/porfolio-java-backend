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
git clone se utiliza principalmente para apuntar a un repositorio existente y clonar o copiar dicho repositorio en un nuevo directorio, en otra ubicación.De manera interna, git clone llama primero a git init para generar un nuevo repositorio. Luego, copia los datos del repositorio existente y extrae un nuevo conjunto de archivos de trabajo.

### _ejemplo_
El sigueinete comando se usa para crear una copia o clonar un repositorio remoto. Se utiliza git clone con la URL de un repositorio.
```
git clone <repo url>
cd my-project 
# Start working on the project

```
## _git config_
El comando git config es una función útil que sirve para definir valores de configuración de Git a nivel de un proyecto global o local. Estos niveles de configuración se corresponden con archivos de texto .gitconfig. Al ejecutar git config, se modificará un archivo de texto de configuración.

### _Niveles y archivos de git config_

El comando git config puede aceptar argumentos para especificar en qué nivel de configuración debe operar. Dispones de los siguientes niveles de configuración.

--local  : La configuración de nivel local se aplica al repositorio de contexto en el que se invoca git config. Los valores de configuración locales se almacenan en un archivo que se puede encontrar en el directorio .git del repositorio: .git/config.

--global : La configuración de nivel global es específica del usuario, lo que significa que se aplica al usuario de un sistema operativo. Los valores de configuración globales se almacenan en un archivo que se encuentra en el directorio principal de un usuario. ~ /.gitconfig en sistemas unix y C:\\.gitconfig en Windows.

--system : La configuración de nivel de sistema se aplica a toda una máquina. Afecta a todos los usuarios de un sistema operativo y a todos los repositorios.
