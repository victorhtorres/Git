# Git

Referencias rápidas de Git.

## Contenido

- [Estados de los archivos en Git.](#Estados-de-los-archivos-en-Git)
    - [Working Directory.](#Working-Directory)
    - [Staging Area.](#Staging-Area)
    - [Git Repository.](#Git-Repository)
- [Configuración básica para trabajar.](#Configuración-básica-para-trabajar)
    - [Correo electrónico.](#Correo-electrónico)
    - [Nombre.](#Nombre)
    - [Configurar editor de texto por defecto.](#Configurar-editor-de-texto-por-defecto)
        - [Configurar Visual Studio Code.](#Configurar-Visual-Studio-Code)
    - [Activar los colores en la terminal para Git.](#Activar-los-colores-en-la-terminal-para-Git)
    - [Más opciones de configuración.](#Más-opciones-de-configuración)
- [Comandos básicos de la terminal.](#Comandos-básicos-de-la-terminal)
    - [Navegación entre directorios.](#Navegación-entre-directorios)
    - [Crea una carpeta.](#Crea-una-carpeta)
    - [Listar contenido de un directorio.](#Listar-contenido-de-un-directorio)
    - [Limpia la terminal.](#Limpia-la-terminal)
    - [Crear archivos.](#Crear-archivos)
    - [Eliminar un archivo.](#Eliminar-un-archivo)
    - [Eliminar carpeta de forma recursiva.](#Eliminar-carpeta-de-forma-recursiva)
- [Creando un repositorio.](#Creando-un-repositorio)
    - [Iniciando un repositorio en un proyecto existente.](#Iniciando-un-repositorio-en-un-proyecto-existente)
    - [Iniciando un repositorio en un nuevo directorio.](#Iniciando-un-repositorio-en-un-nuevo-directorio)
    - [Borrar un repositorio.](#Borrar-un-repositorio)
- [Borrar un repositorio.](#Borrar-un-repositorio)
- [Crear y añadir archivos de nuestro working directory a Staging area.](#Crear-y-añadir-archivos-de-nuestro-working-directory-a-Staging-area)
    - [Devolver un archivo que estaba en staging area al working directory.](#Devolver-un-archivo-que-estaba-en-staging-area-al-working-directory)
    - [Enviar todos los archivos que están en el working directory a staging area.](#Enviar-todos-los-archivos-que-están-en-el-working-directory-a-staging-area)
    - [Eliminar el archivo del staging area y working directory.](#Eliminar-el-archivo-del-staging-area-y-working-directory)
    - [Confirma si un archivo existe o no en nuestro working directory.](#Confirma-si-un-archivo-existe-o-no-en-nuestro-working-directory)
- [Confirmar cambios al repositorio.](#Confirmar-cambios-al-repositorio)
    - [Cambiar mensaje del último commit por otro.](#Cambiar-mensaje-del-último-commit-por-otro)
- [Etiquetando confirmaciones.](#Etiquetando-confirmaciones)
    - [Etiquetas ligeras.](#Etiquetas-ligeras)
    - [Etiquetas anotadas.](#Etiquetas-anotadas)
    - [Otras opciones para las etiquetas.](#Otras-opciones-para-las-etiquetas)
        - [Listar etiquetas creadas.](#Listar-etiquetas-creadas)
        - [Etiquetar commit pasados.](#Etiquetar-commit-pasados)
        - [Borra una etiqueta.](#Borra-una-etiqueta)
- [Revisando historial.](#Revisando-historial)
- [Revisando los cambios entre versiones.](#Revisando-los-cambios-entre-versiones)
- [Reescribir un commit con una versión anterior.](#Reescribir-un-commit-con-una-versión-anterior)
    - [Git reset soft.](#Git-reset-soft)
    - [Git reset mixed.](#Git-reset-mixed)
    - [Git reset hard.](#Git-reset-hard)    
- [Múltiples variantes del repositorio.](#Múltiples-variantes-del-repositorio)
    - [Crear una rama.](#Crear-una-rama)
    - [Listar las ramas creadas.](#Listar-las-ramas-creadas)
    - [Eliminar una rama.](#Eliminar-una-rama)
    - [Renombrar una rama.](#Renombrar-una-rama)
    - [Moverse entre ramas.](#Moverse-entre-ramas)
    - [Crear una rama y navegar en ella.](#Crear-una-rama-y-navegar-en-ella)
- [Mezclando ramas y resolviendo conflictos.](#Mezclando-ramas-y-resolviendo-conflictos)
- [Reescribe la historia de tu proyecto.](#Reescribe-la-historia-de-tu-proyecto)
- [Guardando cambios temporales.](#Guardando-cambios-temporales)
    - [Listar los stash de una rama.](#Listar-los-stash-de-una-rama)
    - [Borra un stash](#Borra-un-stash)
    - [Aplicar el guardado temporal.](#Aplicar-el-guardado-temporal)
- [Cherry pick eligiendo commits selectivamente.](#Cherry-pick-eligiendo-commits-selectivamente)
- [GitHub.](#GitHub)
    - [Clonando repositorios remotos.](#Clonando-repositorios-remotos)
    - [Añadiendo una llave ssh a GitHub.](#Añadiendo-una-llave-ssh-a-GitHub)
    - [Añadiendo un repositorio remoto a uno local.](#Añadiendo-un-repositorio-remoto-a-uno-local)
        - [Listar las conexiones existentes.](#Listar-las-conexiones-existentes)
        - [Eliminar una conexión con algún repositorio.](#Eliminar-una-conexión-con-algún-repositorio)
        - [Traer los archivos que tenga el repositorio remoto al local.](#Traer-los-archivos-que-tenga-el-repositorio-remoto-al-local)
        - [Hacer merge con la rama creada por el fetch y la rama master del local.](#Hacer-merge-con-la-rama-creada-por-el-fetch-y-la-rama-master-del-local)
        - [Traer los cambios del repositorio y hace merge automáticamente con master.](#Traer-los-cambios-del-repositorio-y-hace-merge-automáticamente-con-master)
    - [Enviando cambios al repositorio remoto.](#Enviando-cambios-al-repositorio-remoto)
        - [Enviar todos los tags creados.](#Enviar-todos-los-tags-creados)
        - [Enviar otra rama.](#Enviar-otra-rama)
    - [Proyectos.](#Proyectos)
    - [Creando un template para issues y pull request.](#Creando-un-template-para-issues-y-pull-request)
    - [Ignorando archivos no deseados.](#Ignorando-archivos-no-deseados)
    - [Colabora a proyectos externos.](#Colabora-a-proyectos-externos)
    - [Reportando y monitoreando errores eficientemente.](#Reportando-y-monitoreando-errores-eficientemente)
    - [GitHub Pages hosting gratuito de archivos estáticos.](#GitHub-Pages-hosting-gratuito-de-archivos-estáticos)
    - [Dominios personalizados en GitHub.](#Dominios-personalizados-en-GitHub)


## Estados de los archivos en Git

Git cuenta con 3 estados en los que podemos localizar nuestros archivos:

### Working Directory

El lugar donde se trabajan los archivos.

### Staging Area

El área de preparación de los archivos que serán registrados en el repositorio.

### Git Repository

El lugar donde se almacena el código de forma segura.

## Configuración básica para trabajar

Datos básicos para configurar:

### Correo electrónico

`git config --global user.mail micorreo@xxxx.com`

### Nombre

`git config --global user.name "Tu nombre acá"`

### Configurar editor de texto por defecto

`git config --global core.editor "nombre_app --wait"`

#### Configurar Visual Studio Code

`git config --global core.editor "code --wait"`

### Activar los colores en la terminal para Git

`git config --global color.ui true`

### Más opciones de configuración

Todas las opciones de configuración [aquí](https://git-scm.com/docs/git-config).

## Comandos básicos de la terminal

### Navegación entre directorios

`cd ruta`

### Crea una carpeta

`mkdir nombre_carpeta`

### Listar contenido de un directorio

`ls`

### Limpia la terminal

`clear`

### Crear archivos

`touch nombre_archivo`

### Eliminar un archivo

`rm nombre_archivo_a_eliminar`

### Eliminar carpeta de forma recursiva

`rm -rf nombre_carpeta`

## Creando un repositorio

### Iniciando un repositorio en un proyecto existente

`git init`

### Iniciando un repositorio en un nuevo directorio

`git init nombre_repositorio`

### Borrar un repositorio

Basta con borrar la carpeta .git de la carpeta raíz del repositorio. Ejemplo:

`rm -rf .git`

## Crear y añadir archivos de nuestro working directory a Staging area

Primer, validar el estado del repositorio:

`git status`

Por lo general, al hacer un git status, aparecerán los archivos que han sido modificados en el working area pero que aún no se han pasado al staging area. Lo siguiente es agregar dichos cambios al staging area:

`git add nombre_archivo_agregar`

### Devolver un archivo que estaba en staging area al working directory

`git rm --cach nombre_archivo`

### Enviar todos los archivos que están en el working directory a staging area

`git add -A`

### Eliminar el archivo del staging area y working directory

`git rm -f nombre_archivo`

### Confirma si un archivo existe o no en nuestro working directory

`git add -n nombre_archivo`

## Confirmar cambios al repositorio

Confirma los cambios que tengamos en staging area:

`git commit -m "comentario sobre el cambio"`

Lo anterior, se asegura que los cambios realizados queden guardados en el repositorio.

Para el mensaje del commit, se pone brevemente lo que se está entregando.

### Cambiar mensaje del último commit por otro
    
`git commit --amend -m "comentario"`

Ver el historial de commit:

`git log`

## Etiquetando confirmaciones

Se puede colocar una etiqueta a un commit. Normalmente, se utiliza para colocar el número de la versión de entrega.

Existen dos tipos de etiquetas: Etiquetas ligeras y etiquetas anotadas.

### Etiquetas ligeras

`git tag nombre_etiqueta`

### Etiquetas anotadas

`git tag -a nombre_etiqueta -m "comentario"`

### Otras opciones para las etiquetas

#### Listar etiquetas creadas

`git tag -l`

#### Etiquetar commit pasados

Para etiquetar commit pasados, se requiere conocer el sha-1 del commit el cual se desea etiquetar. Para lo anterior, puede usar el comando `git log` y obtener el sha-1 del commit de interés. Luego, ejecutar el siguiente comando:

`git tag 0.3 sha-1`

#### Borra una etiqueta

`git tag -d 1.0`

*Renombrar una etiqueta*

`git tag -f -a 0.1 -m "comentario del cambio" sha-1`

## Revisando historial

Mostrar histórico de commits:

`git log`

Mostrar histórico de commits de forma mas resumida:

`git log --oneline`

Mostrar el historial con las posibles bifurcaciones que ha tenido:

`git log --oneline --graph`

Mostrar el histórico del último commit:

`git log -1`

## Revisando los cambios entre versiones

Muestra las diferencias entre el commit actual contra el sha-1 del commit ingresado:

`git diff sha-1`

Muestra las diferencias entre dos commits por medio de su sha-1:

`git diff sha-1 sha-1`

Lo anterior también funciona con etiquetas en vez de sha-1.

Nota: Tener en cuenta el orden de los parámetros:

`git diff version_1 version_2`

## Reescribir un commit con una versión anterior

Advertencia: Con este comando puedes perder cosas de tu proyecto.

Hay tres tipos de reset:

git reset [--soft --mixed --hard]

### Git reset soft

Quita un cambio pero lo mantiene en staging area. Deja el header hasta el sha-1 ingresado como parámetro:

`git reset --soft sha-1`

### Git reset mixed

Quitar los commit hasta el sha ingresado como parámetro y también los quita del stage, dejándolo en el working directory:

`git reset --mixed sha-1`

### Git reset hard

Regresa hasta el commit del sha-1 ingresado. Borra todo, incluyendo lo que está en working directory:

`git reset --hard sha-1`

Para recuperar todo, se ingresa el commit el cual tiene los cambios que reestablezca todo lo borrado con reset hard.

## Múltiples variantes del repositorio

### Crear una rama

`git branch nombre_rama`

### Listar las ramas creadas

`git branch -l`

### Eliminar una rama

`git branch -d nombre_rama`

### Renombrar una rama

`git branch -m nombre_rama_actual nombre_rama_nueva`

### Moverse entre ramas

`git checkout nombre_rama`

También se puede usar para moverse entre los commits:

`git checkout sha-1`

### Crear una rama y navegar en ella

`git checkout -b nombre_rama`

## Mezclando ramas y resolviendo conflictos

Ubicarse en la rama donde desea realizar merge. Por lo general, será la rama master quien se mezcle con otros commits.

`git checkout master`
`git merge nombre_rama`

Cuando la mezcla es de tipo **fast-forward**, es porque la rama que se mezcló, venía de la rama master y no han hecho merge con otra rama.

Cuando la mezcla es de tipo **Recursive**, es porque antes del merge realizado, ya hubo uno el cual se mezcló con éxito con la rama master y Git optó por usar otro método para mezclar.

Cuando aparecen conflictos, se debe decidir con que versión quedarse o se debe modificar manualmente la versión conflictiva y luego agregar los cambios al **Staging area** para su posterior confirmación con un commit.

## Reescribe la historia de tu proyecto

Existe otra forma de realizar merge entre ramas, se llama reorganización (rebase), el cual tendrá un comportamiento secuencial, sin bifurcaciones en la linea de tiempo como sucede con el comando git merge. 

`git checkout nombre_rama_a_reorganizar`
`git rebase nombre_rama_a_mezclar`

Al usar rebase, el sha-1 del HEAD cambia. Por lo anterior, se recomienda hacerlo solo en local, porque podría reescribir la historia de todos los que podrían estar contribuyendo con el repositorio de forma remota.

## Guardando cambios temporales

Es un estado intermedio entre un git add y git commit. La idea es guardar temporalmente los cambios agregados al repositorio pero sin confirmarlos:

`git stash` 

### Listar los stash de una rama

`git stash list`

### Borra un stash

`git stash drop nombre_stash`

### Aplicar el guardado temporal

`git stash apply nombre_stash`

## Cherry pick eligiendo commits selectivamente

Se debe ubicar en la rama donde se quiere agregar el commit que estaría en otra rama, por medio de su sha-1:

`git cherry-pick sha-1`

## GitHub

### Clonando repositorios remotos

Lo siguiente, clona un repositorio remoto a local:

`git clone url_repo`

En GitHub existe la opción **fork**, para hacer una copia de un repositorio de otro usuario y poder modificarlo sin afectar el proyecto original.

### Añadiendo una llave ssh a GitHub

Crear la llave:

`ssh-keygen -t rsa -b 4096 -C "correo_registro_en_GitHub"`

Copiar la llave creada:

`cat ~/.ssh/id_rsa.pub`

Con la llave copiada, ir a la cuenta de GitHub > Personal Settings > SSH and GPC keys > New SSH key.

Con la configuración lista, no será necesario introducir usuario y clave cada vez que se envíe una nueva confirmación al repositorio remoto.

### Añadiendo un repositorio remoto a uno local

Conectar un repositorio con nuestro equipo local:

`git remote add origin url_repo_o_ssh`

Nota: La palabra origin significa el nombre del repositorio remoto y se llama así por convención, pero se puede llamar como uno quiera.

#### Listar las conexiones existentes

`git remote -v`

#### Eliminar una conexión con algún repositorio

`git remote remove origin`

#### Traer los archivos que tenga el repositorio remoto al local

`git fetch origin master`

#### Hacer merge con la rama creada por el fetch y la rama master del local

`git merge origin/master --allow-unrelated-histories`

#### Traer los cambios del repositorio y hace merge automáticamente con master

`git pull origin master`

### Enviando cambios al repositorio remoto

`git push origin master`

#### Enviar todos los tags creados

`git push origin master --tags`

#### Enviar otra rama

`git push origin nombre_rama`

### Proyectos

En GitHub, la opción Proyectos, permite organizar las tareas de un repositorio por medio de la metodología Kanban. Se recomienda crear un proyecto por cada confirmación (commit) grande en el repositorio.

**Columnas básicas en un proyecto**

TODO: Son las cosas por hacer.
WIP: Work in Progress. En que estamos trabajando.
Bugs: Cosas que hay que arreglar de manera prioritaria.
Waiting for review: Sirve cuando se trabaja pulls requests, ya que se espera que alguien revise el codigo.
Done: Cuando la tarea ha finalizado.

### Creando un template para issues y pull request

GitHub permite usar templates a la hora de generar un Pull Request o Issues en nuestro repositorio:

**Pull request**

En el repositorio, crear un archivo llamado pull_request_template.md y definir los lineamientos en Markdown.

**Issues**

En el repositorio, crear un archivo llamado issue_template.md y definir los lineamientos en Markdown.

Cada vez que alguien vaya a generar un Issues o Pull request en el repositorio, GitHub le cargará por defecto el templado que hemos definido.

### Ignorando archivos no deseados

Crear un archivo en el repositorio llamado .gitignore . Lo anterior, sirve para que los nombres de archivos agregados en .gitignore, el sistema git los ignore y así no los envíe a un repositorio remoto.

### Colabora a proyectos externos

Un *Pull Request* es una solicitud para que el dueño del repositorio realice los cambios que estas proponiendo. Estos nunca se hacen a la rama master, para evitar inconvenientes.

**Consideracioens**

1. Si eres el dueño del repositorio, debes protejer la rama master, para que siempre alguien externo, pida permiso, para hacer aportes al repositorio. Lo anterior evita que se puedan hacer inyecciones de cambios de manera directa, sin una supervisión.

2. Hacer un template dónde, el que va a hacer el aporte, detalle aquellas modificaciones que realizo. Lo anterior, agiliza el flujo colaborativo y optimiza los procesos de producción de software.

### Reportando y monitoreando errores eficientemente

Issues: Sirve para reportar un problema o sugerir algún cambio para el repositorio.

Milestones: Forma para agrupar Issues o Pull Request.

### GitHub Pages hosting gratuito de archivos estáticos

Ir a settings > GitHub Pages y eliges la rama gh-pages o master y guardas. Ya tendras tu pagina subida a un hosting gratuito de GitHub.

Nota: Solo se permite páginas estáticas.

### Dominios personalizados en GitHub

En settings, en la opción GitHub pages, configurar el dominio personalizado. Pedirá crear un archivo llamado CNAME en el repositorio. Dentro del archivo colocar el nombre del dominio.

También, se requiere configurar del lado de la gestión de dominio, los CNAMES y records del dominio, para que apunte al repositorio en GitHub y esto varia con base al proveedor de dominios.

Más información [aquí](https://help.GitHub.com/en/articles/using-a-custom-domain-with-GitHub-pages)