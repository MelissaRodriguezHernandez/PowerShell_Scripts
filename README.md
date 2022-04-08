# PowerShell Scripts

> Esta práctica tiene el objetivo de analizar y documentar una serie de scripts de PowerShell

## Requisitos previos

Powershell tiene restringida la ejecución de scripts para asegurar la seguridad de la máquina y prevenir ataques maliciosos. Debido a esto tendremos que configurarlo.

Con el código siguiente podremos saber el estado de las restricciones:

~~~
Get-ExecutionPolicy
~~~

![ver estado](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/ver%20estado.png)

Si el resultado nos dice 'restricted' significa que está limitado, para quitar esas limitaciones usaremos el siguiente comando:

~~~
Set-ExecutionPolicy Unrestricted
~~~

![](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/cambiar%20estado.png)

## Script 1

[Enlace al archivo](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/Scripts/1.ps1)

~~~
.\1.ps1
~~~

Descripción: 
Se declaran una variable llamada *number*, se le asigna diferentes valores y se saca por pantalla por cada valor.

Resultado :

![resultado script 1](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script1.png)

## Script 2

[Enlace al archivo](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/Scripts/2.ps1)

~~~
.\2.ps1
~~~

Descripción:

Primera parte. Tenemos una variable integer que tiene asignado un número, y a través de una iteración de tipo *for* se irá imprimiendo por pantalla *hello* la cantidad igual al número asignado a esa variable.

Segunda parte. Seguimos teniendo una variable de tipo integer y a través de un bucle se ira imprimiendo por pantalla *hello* el número de veces que hemos asignado.

Tercera parte. Es casi igual al anterior pero en este caso le sumamos un *do* al *while*.

(Estas tres primeras partes representan los 15 *hello* que salen por pantalla)

Cuarta parte. Se declara en una variable de tipo *String* el texto *PowerShell for Beginners*, y a través del bucle *foreach* se va imprimiendo por pantalla letra por letra el String antes declarado.

Quinta parte. Volvemos a declarar una variable de tipo *String* con el mismo contenido de la parte anterior, y, a través de comandos concatenados sacamos por pantalla el contenido letra por letra.

Resultado:

![resultado script parte 1](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script2.png)

![resultado script parte 2](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script%202%20parte%202.png)

## Script 3

[Enlace al archivo](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/Scripts/3.ps1)

~~~
.\2.ps1
~~~

Descripción: 

Este script nos demuestra la importancia de definir bien el tipo de variable que usamos. 
También contiene una pequeño juego al final con diferentes opciones que nos dará distintos resultados según nuestra elección (left, right).

Resultado: 

![script 3 primera parte](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script%203%20parte%201.png)

Si introducimos *left*

![script 3 left parte 1](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script%203%20left%20parte%201.png)

![script 3 left parte 2](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script%203%20left%20parte%202.png)

Si introducimos *right*

![script 3 right parte 1](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/Script%203%20right%20parte%201.png)

![script 3 right parte 2](https://github.com/MelissaRodriguezHernandez/PowerShell_Scripts/blob/main/img/script%203%20right%20parte%202.png)
