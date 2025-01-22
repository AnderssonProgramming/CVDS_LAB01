# LABORATORIO 1- INTRODUCCIÓN GIT
ESCUELA COLOMBIANA DE INGENIERÍA - CICLOS DE VIDA DE DESARROLLO DE SOFTWARE

 ![alt text](assets/image.png)


  
## PARTE I (Trabajo Individual). 

1.	Crea un repositorio localmente.

    ![alt text](assets/image-3.png)

2.	Agrega un archivo de ejemplo al repositorio, el **README.md** puede ser una gran opción.

    ![alt text](assets/image-4.png)

3.	Averigua para qué sirve y como se usan estos comandos **git add** y **git commit -m “mensaje”**

    ### **git add** = Mueve los cambios del directorio de trabajo al área del entorno de ensayo.
    ### **git commit -m "mensaje"** = captura una instantánea de los cambios preparados en ese momento del proyecto.

4. Abre una cuenta de github, si ya la tienes, enlazala con el correo institucional.
   
  ![alt text](assets/image-1.png)
   
5.	Crea un repositorio en blanco (vacío) e GitHub.

![alt text](assets/image-2.png)
   
6.	Configura el repositorio local con el repositorio remoto.

      [Como subir un proyecto local a github.](https://gist.github.com/cgonzalezdai/cc33db72a6fe5178637aabb562eae35c)

      ![alt text](assets/image-9.png)
  
7.	Sube los cambios, teniendo en cuenta lo que averiguaste en el punto 3
    Utiliza los siguientes comando en el directorio donde tienes tu proyecto, en este orden:
   	```bash
      git add .
    ```

    ![alt text](assets/image-5.png)
    ```bash
      git commit -m "mensaje, lo que hiciste con el archivo"
    ```
    ![alt text](assets/image-6.png)

    ```bash
     git config user.name "Nombre del usuario"
    ```
    ![alt text](assets/image-7.png)
    ```bash
      git push "url repositorio"
    ```

    ![alt text](assets/image-8.png)

8.	Configura el correo en git local de manera correcta
     [Configurar correo electrónico en GitHub](https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)

     ![alt text](assets/image-11.png)
9.	Vuelve a subir los cambios y observa que todo esté bien en el repositorio remoto (en GitHub).

    ![alt text](assets/image-12.png)
    ![alt text](assets/image-13.png)


## PARTE II (Trabajo en parejas)

1.	Se escogen los roles para trabajar en equipo, una persona debe escoger ser "Owner" o Propietario del repositorio y la otra "Collaborator" o Colaborador en el repositorio.
   
   ![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/716464e4-d663-477d-a87d-0f2944e5b709)

   ### Owner = Cristian Pedraza 
   ### Collaborator = Andersson Sánchez

2.	El owner agrega al colaborador con permisos de escritura en el repositorio que creó en la parte 1
   
     [Invitar colaboradores a un repositorio personal](https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository)
    
    Cristian me agrega como colaborador al repositorio que él creó.

3.	El owner le comparte la url via Teams al colaborador

    ![alt text](assets/image-14.png)

4.	El colaborador acepta la invitación al repositorio.

![alt text](assets/image-15.png)
*Ahora ya tengo acceso al repositorio de Cristian*
![alt text](assets/image-16.png)

*Hago git clone para bajar el repositorio central de Cristian de manera local en el computador.*
![alt text](assets/image-17.png)

![alt text](assets/image-18.png)
5.	Owner y Colaborador editan el archivo README.md al mismo tiempo e intentan subir los cambios al mismo tiempo.
6.	¿Que sucedió?

![alt text](assets/image-20.png)
![alt text](assets/image-19.png)
7.	La persona que perdió la competencia de subir los cambios, tiene que resolver los conflictos, cúando haces pull de los cambios, los archivos tienen los símbolos `<<<` `===` y `>>>` (son normales en la resolución de conflictos), estos conflictos debes resolverlos manualmente.
         [Como resolver Conflictos GitHub](https://docs.github.com/es/enterprise-cloud@latest/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)
         

![alt text](assets/image-21.png) 
*Se resolvieron los conflictos dándole en resolve merge*
![alt text](assets/image-22.png)
8.	Volver a repetir un cambio sobre el README.md ambas personas al tiempo para volver a tener conflictos.
  
  *Ahora yo hago push y luego mi compañero el pull para ver el error que sucede para solucionarlo en IntellijIDEA*

  ![alt text](assets/image-23.png)


9.	Resuelvan el conflicto con IntelliJ si es posible,  [Resolver conflictos en IntelliJ]( https://www.jetbrains.com/help/idea/resolving-conflicts.html#distributed-version-control-systems)

De esta forma ya sabes resolver conflictos directamente sobre los archivos y usando un IDE como IntelliJ, esto te será muy útil en los futuros trabajos en equipo con Git.

## PARTE III (Trabajo de a parejas)
1.	¿Hay una mejor forma de trabajar con git para no tener conflictos?

Si, esa forma consiste en no trabajar todo sobre el repositorio central, sino crear una rama nueva, y sobre esa hacer cambios, luego cuando esté seguro que el proyecto está bien, entonces se hace el PR, para subir y dejar todo en la rama principal (main); usando git flow.

2.	¿Qué es y como funciona el **Pull Request**?

Permite a tu equipo solicitar la revisión y aprobación de sus cambios antes de fusionarlos en la rama principal (main).


3.	Creen una rama cada uno y suban sus cambios
   
   ![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/e558ac3b-f5d8-443a-8958-aacdedef7f94)
  	![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/074eacc9-6284-4a41-9805-c9e30a169e5d)
  	![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/5c664e91-d3a3-4b56-867b-3b06d9ffce72)


  ![alt text](assets/image-24.png)
  
4.	Tanto owner como colaborador hacen un cambio en el README.md y hacen un Pull Request (PR) a la rama main/master
   
     [Pull Request - GitHub](https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
  	
   
 **(Recomendación : deben trabajar en equipo y distribuirse de mejor manera quien va a modificar qué, para evitar modificar los mismos archivos al mismo tiempo, si no se editan los mismos archivos la resolución de conflictos es automática)**

5.	Teniendo en cuenta la recomendación, mezclen los cambios a la rama main a través de PR con el check/review/approval del otro compañero (Cuando se hace merge se deberían borrar las ramas en github)

***Como Borrar Ramas después de un Pull Request***

Se dirigen a la configuración de su repositorio:

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/859fb07c-5748-4b8e-91f4-2f5ee7229f90)

Y en general

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/a2bc8b9d-4200-472e-a712-56498b0f59b3)

Se dirigen al final en el área del pull requests y seleccionan “Automatically delete head branches”

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/838f51a7-6b2c-4673-9a60-65fe11a75647)

***Aprobación Pull Request***

Nos dirigimos (todavía en configuraciones) a Branches, en esta visualizarán donde daremos protección de nuestras ramas, seleccionamos Add rule

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/7104fcaa-c1dd-4345-a8d0-d6a4f531de79)

Aquí damos el nombre de nuestra rama (Verificar el nombre tal cual lo tenemos en nuestro repositorio) y seleccionamos la primera opción como se muestra, así estamos requiriendo que cuando se haga ese pull request en nuestra rama se necesita aprobación de otro compañero

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/0631402e-6210-4b8a-a040-de594455e3b0)

Vamos al final y damos clic en Create

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/7e878bd7-8b68-4403-af98-380700d81459)

Y así protegimos nuestra rama principal, esto se vuelve muy relevante cuando trabajamos en parejas o en equipos, deberían tener un mensaje final que se vea así

![assets/image](https://github.com/PDSW-ECI/labs/assets/118181543/1e39b81c-82c8-4fec-b2e6-b339c782b6ad)


## ENTREGA
- En un README.md colocar lo siguiente:
- Una sección llamada “INTEGRANTES” y allí colocar el listado de los integrantes del taller (máximo 2).
- Una sección llamada “RESPUESTAS” colocar las respuestas a las preguntas.
- La entrega deberá realizarla en Moodle en el espacio correspondiente a su grupo.