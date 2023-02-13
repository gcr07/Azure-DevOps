# Azure-DevOps
Azure DevOps to DevSecOps


![image](https://user-images.githubusercontent.com/63270579/217354187-e6169d30-eb20-44f2-bbc4-29c5c558ea21.png)

## Azure repos 

Es un repositorio de GIT nada mas donde podemos tener el codigo no hay que complicarse.

## Azure pipelines 

Son como una especie de scripts donde defines tareas ( por ejemplo escanear el codigo con sonar por ejemplo) Continue integration CI continue Delivery CD.
Existen disparadores que pueden configurarse un ejemplo es un commit en un repo.

## Azure Artifacts

Supongamos que se crea una libreria aqui se guarda y pues se usa cuando se vaya a compilar guarda artefactos.

## Azure Boards 

Como mas administrativo.

## Azure Test Plans

Igual mas administrativos

## Extension y marketplace

Por ejemplo son extenciones como sonar cloud para escanear codigo etc.

## Para poder ejecutar un pipeline

Para poder usar paralel jobs microsoft protegio sus servidores y ahora tienes que hacer un request para que te permitan usar los pipelines.

> https://learn.microsoft.com/en-us/azure/devops/pipelines/licensing/concurrent-jobs?view=azure-devops&tabs=ms-hosted

## Seguridad

![image](https://user-images.githubusercontent.com/63270579/217894503-1932f874-fe07-44ed-87b0-f1f502c9dece.png)

Por el lado derecho y como rama principal tenemos la organizacion despues tenemos cada proyecto dentro de esa organizacion. Usualmente los permisos se otorgan atravez de grupos aunque se le puede dar a un usuario en particular


## Project collection

Todos los proyectos que se pueden crear dentro de la organizacion. Todos los usuarios que esten dentro de este grupo podran ver todos los proyectos.


# Git Metodologias

![image](https://user-images.githubusercontent.com/63270579/218518048-fc7c0899-c60c-4acd-8bf0-6ab38c6479f6.png)


## GIT

Lo importante que hay que recordar es que git la rama no se llama master si no ya esta como main entonces solo cambia cuanod instales.

## Token 

![image](https://user-images.githubusercontent.com/63270579/218222092-631234cc-b94f-47cc-8101-0ac978952cca.png)

Para que el cliente de windows de git se pueda comunicar usa un token. Se usaron los comandos para configurar localmente 

```

git config --global user.name "Ger"

git config --global user.email "truco_"

git config --global credential.helper cache


Para borrar la cache en caso de equivocacion 

git config --global --unset credential.helper 

```


## Crear un repo (localmente) 

En este caso ya bajamos el commons.zip que tenia un proyecto en JAVA

```

git init

git add .

 git commit -m "First commit"

 git branch
 
 ```
 
 ### crear en azure el repo
 
Estos pasos se crearon antes osea es del video el escenario es: supuesto que tu estas poniendo el repo que creaste le dices que ahora el origen sera el repo de azure para que localmmente y en azure esten alineados.

```

 git remote add origin https://Suko9@dev.azure.com/Suko9/MyFirstProject/_git/common

git push -u origin --all ## todos los cambios los mandamos al nuevo origin 


```

## Para traernos los cambios

en uestra consola de visual code ( osea en la carpeta ahi hacemos  un pull)

```
git pull origin

```


## Aplicamos la metodologia git flow 

Creamos una rama develop en base a la rama main

```
git branch develop main

git branch # Sirver para ver todas las branchs que tenemos

```







































