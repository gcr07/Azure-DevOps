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


## GIT

Lo importante que hay que recordar es que git la rama no se llama master si no ya esta como main entonces solo cambia cuanod instales.

## Token 

![image](https://user-images.githubusercontent.com/63270579/218222092-631234cc-b94f-47cc-8101-0ac978952cca.png)

Para que el cliente de windows de git se pueda comunicar usa un token.












































