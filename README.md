
# Actividad 1

> # Datos personales
>
>> ## Nombre Completo
>>
>> Patricio Estrada Carreto
>>
>> ## Matrícula
>>
>> AL02856588
>>
>> ## Carrera
>>
>> Ingeniería en Desarrollo de Software (IDS)
>>
>> ## Semestre
>>
>> 6° Semestre (Enero - Mayo 2023)
 
 ***
 
> # Información del curso
>>
>> ## Nombre de la materia
>>
>> Diseño de Aplicaciones Web
>>
>> ## Instructor de la materia
>>
>> Erik Carrillo Moo

 ***
 
> # ¿Para que se usa Markdown?
> Se trata de un lenguaje que permite crear texto con formato el cual se le puede dar si se colocan ciertos caracteres especiales detras o incluso rodeando los parrafos que deben tener la presentación deseada. Se trata de un lenguaje muy similar a HTML5, siendo que los caracteres especiales reemplazan a las etiquetas. A su vez comparten ciertos elementos, como la capacidad de poner encabezados, hacer listas, insertar lineas, colocar el texto en *itálicas*, **negritas** o inclusive ***ambas***, etc..
> 
> De manera personal, puedo concluir que Markdown es una herramienta útil que permite realizar un trabajo similar a HTML5 utilizando una sintaxis mucho mas amigable a comparación de esta última, aunque claro, con las mismas limitaciones.

 ***

# Tarea 1

## Etiquetas de Markdown mas comunes

|Etiqueta|Sintaxis|Descripción|
|:----:|:----:|----|
|Encabezados|```# (Texto)```|Se utiliza para dar el formato de encabezado a texto normal, el número de Hashtags (#) determina la prioridad de encabezado que tiene (menos #, mayor prioridad y tamaño).|
|Énfasis|```*(texto)*```|Resalta una parte del texto sobre el resto, dependiendo de la cantidad de asteristicos que rodeen la cadena, el tipo de enfasis cambia. (1 par es *itálicas*, 2 son **negritas** y 3 son las 2 anteriores ***juntas***).|
|Listas no numeradas|```* (Texto)```|Hace que la linea siguiente pertenezca a una lista no numerada.|
|Listas enumeradas|```(Numero). (Texto)```|Hace que la linea siguiente pertenezca a una lista enumerada, aplicar sangría a cualquiera de las 2 clases de lista modifica la jerarquía del elemento.|
|Hipervinculos|```[Texto](Enlace)```|Hace que el texto encerrado en los corchetes actué como enlace a la página con el hipervinculo especificado después.|

## Comandos de git mas importantes

### git status

Este comando permite mostrarle al usuario la situación actual del repositorio local que se encuentra abierto, mostrando las acciones qe se han hecho dentro del mismo, ya sea para indicar archivos nuevos o modificados, al igual que para verificar si dichos cambios ya se encuentran añadidos dentro de la pila de temporal.

    $ git status

### git add

Este comando añade a la pila de cambios a guardar el archivo especificado.

    $ git add <nombreDeMiArchivo>
    
> Si se desean añadir todos los archivos nuevos/modificados a la pila de cambios a guardar a la vez, se puede usar el siguiente parametro con el mismo comando
>
>   ```
> $ git add -A

### git commit

Este comando permite guardar dentro del repositorio una versión del proyecto con todos los cambios registrados en la pila de cambios previamente, adicionalmente se le coloca un mensaje que describa brevemente la versión creada del proyecto.

    $ git commit -m "<Texto>"
    
### git push

Con este comando se pueden mandar los archivos de un repositorio local a su repositorio remoto respectivo. Para ello, es necesario tener en cuenta la *branch* que se desea subir al repositorio al igual que el nombre que se tiene guardado para referirse al repositorio remoto, (el cual normalmente es "origin").

    $ git push <nombreRepositorioRemoto> <branchAMandar>

### git checkout

Este comando permite cambiar de *branches*, siempre y cuando la *branch* a la cual cambiarse sea una que ya existe en el repositorio local.

    $ git checkout <nombreDeBranchExistente>
    
> Si se desea crear una nueva *branch* y cambiarse a ella, se debe realizar el mismo comando utilizando un parametro de por medio
>
>   ```
$ git checkout -b <nombreDeBranchNueva>

### git branch --delete

Este comando en particular permite poder eliminar la *branch* especidficada posteriormente.

    $ git branch --delete <nombreBranchABorrar>
    
### git revert

Este comando se encarga de generar un nuevo commit posterior al último commit que contenga la versión del repositorio especificada por el *hash* que haga referencia al mismo, de este modo regresando a una versión anterior del proyecto sin la necesidad de modificar el historial del mismo.

    $ git revert <hashDelCommitARevertir>
