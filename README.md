#### GH PAGE: https://biokah.github.io/twitter/

### Twitter
Reto de código. Unidad "Creando interacción con JavaScript"
Objetivo: Recrear la página Twitter con los puntos de funcionalidad requeridos en LMS.

### Solución:
#### Maquetado de HTML:
Creación de una estructura con dos una sección superior e inferior. La superior a su vez está dividida en dos. La sección superior izquierda simula la sección que incluyen los datos personales del perfil en Twiiter. Por otro lado, la sección superior derecha es la textarea donde el usuerio ingresa el texto que desea publicar. El botón Submit que contiene la funcionalidad. 
La parte inferior es la sección donde se publican los twitts que ha ingresado el usuario. Según el orden, los twitts más nuevos se imprimen en la parte superior. 


#### Lógica de JavaScript
- Imprimir Tweet. Al ejecutar el evento submit, se ejecutarán la funcion:

    i. Crear elementos de tweet enviado (div que contiene un p y span)

    ii. Obtener hora. Se usará otra función.

    iii. "Unir" los elementos creados para obtener estructura arquitectada.

    iv. El boton de submit estará deshabilitado por default. Al ejecutar esta función se habilitará y cambiara de color.
    v. Prevenir Default para que el evento no provoque que la página se reinicie.

- Imprimir contador de caracteres restantes en tweet. Default 140. La funcion se ejecutara con el evento keyup

    i. Obtener los caracteres del texto ingresado en la textarea.

    ii. Imprimir en span contador la resta de default caracteres y el largo de caracteres ingresados.
Para hacer que el contador indique visualmente (colorres) los caracteres restantes, se usará un if y al llegar de 120 a 130 caracteres se pintara amarillo el contador, de 130 a 140 se pintará rojo.
    
    iii. Al llegar a 140 caracteres el boton submit se deshabilitara
- Obtener hora de tweet

De las funciones getHours y getMinutes separar por horas y minutos
- Reestablecer tamaño de textarea despues de enviar el tweet. Lo accionará evento input.

    i. Por medio de asignacion de estilo, se asignará el height default al textarea.

##### Funcionalidades adicionales:
Página responsiva mediante uso de grids