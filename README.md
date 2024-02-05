        Juan Felipe Rubio Sanabria J1

    Ejercicio 1:

-Esta trabajando en un proyecto Git colaborativo con varias ramas y commits. Tu tarea es
utilizar el comando git log con algunas opciones específicas para obtener un resumen
gráfico de los últimos 5 commits en todas las ramas.

utilice el --max-count=5 : Esto genera el numero especifico de commits que se mostrara.

    Ejercicio 2:

-Esta trabajando en un proyecto Git colaborativo y necesitas obtener una visión gráfica y
detallada del historial de commits. Tu tarea es utilizar el comando git log con opciones
específicas para personalizar el formato y presentación de la salida. La salida debe tener
las siguientes especificaciones:

Muestra una representación gráfica del historial de commits

Muestra el hash corto del commit en color rojo

Muestra las referencias (ramas o tags) en las que está involucrado el commit en color
amarillo

Muestra el mensaje del commit.

Muestra la fecha relativa del commit en color verde.

Muestra el hash del commit como un identificador abreviado.

Muestra las fechas de los commits de forma relativa

Utilice los siguientes codigos:
- git log --graph --abbrev-commit --decorate --pretty=format:'%C(red)%h %C(yellow)%d %C(white)%S %s %C(green)%ar'

    Explicacion:

graph: Muestra una representación gráfica de todo el commits.

abbrev-commit: Muestra unicamente la version abreviada del hash del commit.

decorate: Muestra las ramas y tags junto a los commits.

%C(red):Genera el color del siguiente texto.

%h: Muestra el hash corto del commit.

%C(yellow): Genera el color del siguiente texto.

%d: Muestra las referencias como lo son las ramas y las tags.

%C(white): Genera el color del siguiente texto.

%s: Muestra el mensaje del commit

%C(green): Genera el color del siguiente texto.

%ar: Muestra la fecha del commit

    Ejercicio 3:

Estas trabajas frecuentemente con el comando git log -1 HEAD para obtener detalles sobre
el último commit en la rama actual. Sin embargo, encuentras que escribir este comando
completo es un poco tedioso. Quieres simplificarlo creando un alias personalizado.

Tu tarea es utilizar el comando git config para crear un alias llamado last que represente el
comando git log -1 HEAD.

git config --global alias.last "status --short"

git config --global: Establece la configuración global de git

alias.last: Le nombre que se le pone a alias.

"status --short": permite visualizar un resumen con flag que indica el estado de los archivos.

    Ejercicio 4: 

Imagina que deseas simplificar el proceso de editar la configuración global de Git. Tu tarea
es utilizar el comando git config para crear un alias que te permita abrir fácilmente la
configuración global en tu editor de texto preferido. Ejecuta el comando para crear un alias
llamado ec que cumpla con la especificación dada.

Utilice los siguientes codigos:

    git config --global alias.ec "config --global core.editor 'code -wait'" git ec

git config --global: Establece la configuración a nivel global.

alias.ec  Crea un alias llamdo ec

config --global core.editor 'code -wait" -> Configura el editor establecido como Visual Studio Code con el codigo `-wait

    Ejercicio 5:

Imagina que estás trabajando en un proyecto Git colaborativo con múltiples colaboradores
y ramas. Tu tarea es utilizar el comando git log con opciones específicas para personalizar
la salida del historial de commits y resaltar información clave.

Utilice los siguientes codigos:

    git log --graph --abbrev-commit --decorate --pretty=format:'%C(yellow) %h/ %C(red)/%d %C(white) %S %s %C(blue)/ %an'

graph: Muestra una representación gráfica de todo el commits.

abbrev-commit: Muestra un hash de commit abreviado.

decorate -> Muestra las referencias (ramas y tags) en el historial.

pretty=format -> Personaliza el formato de salida del historial de commits.

%C(yellow): Genera el color del siguiente texto.

%h; Muestra el hash corto del commit.

%C(red): Genera el color del siguiente texto.

%d: Muestra las referencias como lo son las ramas y las tags.

%C(white): Genera el color del siguiente texto.

%S: Muestra el nombre del firmante del commit.

%s: Muestra el mensaje del commit.

%C(blue): Genera el color del siguiente texto.

%an: Muestra el nombre del autor del commit.
