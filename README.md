# actividad_Git
**1. investigación básica de Git:** <br>
a.<br>
1_ Git es un sistema de control de versiones distribuido que localiza los cambios en cualquier conjunto de archivos de computadora, generalmente utilizado para coordinar el trabajo entre programadores que desarrollan código fuente en colaboración durante el desarrollo de software. Sus objetivos incluyen velocidad, integridad de datos y soporte para flujos de trabajo distribuidos y no lineales.

**b. ¿Cuáles son las principales características de Git?**<br>
Las principales características del git son: el control y almacenamiento de cambios, ramificación y fusión, repositorios distribuidos, gestión de conflictos, historial y etiquetado, velocidad y rendimiento, flexibilidad y escalabilidad, y compatibilidad con diversas plataformas.

**c. ¿Qué es un sistema de control de versiones?**<br>
Un sistema de control de versiones es una herramienta que registra y controla los cambios en archivos y proyectos. Permite mantener un historial de modificaciones, trabajar en paralelo y colaborar en el desarrollo de software.

**d. ¿Cuál es la diferencia entre Git y otros sistemas de control de versiones?**<br>
**Git almacena la historia completa del proyecto como instantáneas, lo que facilita el acceso rápido a versiones anteriores.
Git deja realizar operaciones sin conexión a un servidor central, lo que nos da flexibilidad y capacidad de trabajar offline.
Git facilita la creación y gestión de ramas, como la fusión eficiente de cambios entre ellas.
Git es escalable y ofrece un rendimiento óptimo en proyectos de cualquier tamaño.
Git cuenta con una amplia comunidad de usuarios y desarrolladores, lo que proporciona recursos y herramientas disponibles.**

**2 Instalación y configuración de Git:**<br>
**a. Investiga cómo instalar Git en diferentes sistemas operativos (Windows, macOS, Linux).**<br>
*Windows:*<br>
-Descargar el instalador de Git desde el sitio web oficial y ejecutarlo.
-Sigue las instrucciones del asistente de instalación, aceptando los ajustes predeterminados.
-Git estará disponible en la línea de comandos y se instalará Git Bash, una interfaz gráfica.
macOS:
-Verifica la instalación ejecutando git --version en la Terminal.
-Si no está instalado, se puede instalar a través de las herramientas de línea de comandos de Xcode.
Linux (Debian/Ubuntu):
-Abre una terminal y actualiza los repositorios de paquetes con sudo apt update.
-Instala Git con sudo apt install git.

b. Explica los pasos para configurar tu nombre de usuario y dirección de correo electrónico en Git.<br>
**-Abrir la terminal.**<br>
-Verifica la configuración actual con el comando 
**git config --global --list.**<br>
-Configurar el nombre de usuario con el comando 
**git config --global user.name "Tu Nombre".**<br>
-Configurar la dirección de correo electrónico con el comando 
**git config --global user.email "tucorreo@example.com".**<br>
-Verificar la configuración actualizada con el comando 
**git config --global --list.**

**3 Comandos básicos de Git:** <br>
***a. Investiga los comandos git init, git add, git commit y git status. Explica qué hacen y cómo se utilizan.*** <br>
**-git init:** Crea un nuevo repositorio de Git en un directorio. <br>
**-git add:** Agrega archivos al área de preparación para incluirlos en el siguiente commit. <br>
**-git commit:** Confirma los cambios realizados en el área de preparación y crea un nuevo commit en el historial del repositorio. <br>
**-git status:** Muestra el estado actual del repositorio, incluyendo los cambios realizados y los archivos en el área de preparación. <br>

**b. Describe los comandos git log y git diff para ver el historial de cambios y las diferencias entre versiones, respectivamente.** <br>
El comando **git log** se utiliza para ver el historial de cambios en un repositorio Git. Muestra una lista cronológica de confirmaciones, con detalles como autor, fecha y mensaje descriptivo. <br><br>
El comando **git diff** muestra las diferencias entre versiones de archivos en un repositorio Git. Puede mostrar diferencias entre el directorio de trabajo y el área de preparación, o entre confirmaciones específicas. Proporciona opciones para mostrar las diferencias de manera más compacta o detallada.


4 Trabajando con repositorios remotos: <br>
a. Investiga cómo clonar un repositorio remoto con git clone. <br><br>
-Abrir una terminal y navegar hasta el directorio deseado. <br><br>
-Obtén la URL del repositorio remoto. <br><br>
Ejecutar git clone <URL> en la terminal, cambiando <URL> con la URL del repositorio. <br><br>
-Tocar el Enter y Git comenzará a clonar el repositorio en tu directorio actual. <br><br>
-Si es necesario, proporciona las credenciales de autenticación. <br><br>
-Una vez completada la clonación, tendremos una copia local del repositorio remoto. <br><br>
b. Explica cómo trabajar con ramas utilizando los comandos git branch, git checkout y git merge. <br><br>
-git branch: Crear, listar o eliminar ramas. <br><br>
git branch nombre-rama: Crea una nueva rama. <br><br>
git branch: Lista las ramas existentes. <br><br>
git branch -d nombre-rama: Elimina una rama. <br><br>
-git checkout: Cambiar entre ramas o crear una nueva rama y cambiar a ella. <br><br>
git checkout nombre-rama: Cambia a una rama existente. <br><br>
git checkout -b nombre-rama: Crea y cambia a una nueva rama. <br><br>
git checkout -- nombre-archivo: Descarta cambios en   un archivo. <br><br>
-git merge: Fusionar cambios de una rama en otra. <br><br>
git merge nombre-rama: Fusiona una rama en la rama actual. <br><br><br>

**b. Explica cómo trabajar con ramas utilizando los comandos git branch, git checkout y git merge.** <br>
-git branch: Crear, listar o eliminar ramas.  <br><br>
git branch nombre-rama: Crea una nueva rama. <br><br>
git branch: Lista las ramas existentes. <br><br>
git branch -d nombre-rama: Elimina una rama. <br><br>
-git checkout: Cambiar entre ramas o crear una nueva rama y cambiar a ella. <br><br>
git checkout nombre-rama: Cambia a una rama existente. <br><br>
git checkout -b nombre-rama: Crea y cambia a una nueva rama. <br><br>
git checkout -- nombre-archivo: Descarta cambios en   un archivo. <br><br>
-git merge: Fusionar cambios de una rama en otra. <br><br>
git merge nombre-rama: Fusiona una rama en la rama actual. <br><br>

**c. Investiga cómo subir tus cambios locales a un repositorio remoto con git push.** <br>
-Realizar y confirmar cambios locales con git commit. <br>
-Verificar la configuración del repositorio remoto con git remote -v. <br>
-Si no vinculaste tu repositorio local al remoto, usa git remote add para agregarlo. <br>
-Utiliza git push <nombre_repositorio_remoto> <rama_local>:<rama_remota> para subir tus cambios. <br>
<nombre_repositorio_remoto> es el nombre del repositorio remoto, como "origin". <br>
<rama_local> es el nombre de tu rama local con los cambios. <br>
<rama_remota> es el nombre de la rama correspondiente en el repositorio remoto. <br>
Git verificará los permisos y posibles conflictos, y subirá tus cambios al repositorio remoto. <br>

**5 Colaboración en Git:**
**a. Investiga cómo trabajar en equipo en un repositorio remoto utilizando ramas y fusiones.**
-Clonar el repositorio remoto: Cada miembro del equipo clona el repositorio remoto en su máquina local. <br>
-Crear y cambiar a una nueva rama: Cada miembro crea una nueva rama para su tarea y se cambia a ella. <br>
-Trabajar en la rama localmente: Los miembros del equipo realizan cambios en la rama específica. <br>
-Subir la rama al repositorio remoto: Los cambios se suben al repositorio remoto. <br>
-Solicitar una fusión (pull request): Se solicita la fusión de la rama en el repositorio remoto.<br> 
-Revisar y discutir los cambios: Los miembros revisan y comentan los cambios propuestos. <br>
-Realizar ajustes y actualizaciones: El autor de la solicitud realiza ajustes en la rama según los comentarios recibidos. <br>
-Fusionar la rama: La rama se fusiona con la rama principal del repositorio remoto. <br>

**b. Explica qué son las solicitudes de extracción (pull requests) y cómo se utilizan para revisar y aprobar cambios.** <br>
***Las solicitudes de extracción son propuestas para fusionar cambios en un proyecto de software. Los desarrolladores crean una solicitud desde una rama con modificaciones hacia la rama principal. Otros revisan el código, hacen sugerencias y plantean preguntas. Después de iteraciones y pruebas, los cambios se aprueban y fusionan en la rama principal. Las solicitudes de extracción mejoran la colaboración y calidad del software antes de la fusión.***

