Training_F1
===========
@author: Victor

Entrenamiento Phyton - Fundamentos

**VERIFICACION DE CUIT/CUIL** (genérico)

El CUIL/CUIT consta de 11 números. Los 10 primeros (2 + 8) constituyen el código de identificación y el último, el dígito de verificación. Para obtener esta verificación se procede de la siguiente forma:

A cada dígito del código, se lo multiplica por los siguientes números (respectivamente) 5, 4, 3, 2, 7, 6, 5, 4, 3, 2 y cada valor obtenido, se suma para obtener una expresión (que llamaremos "valor 1").

A este "valor 1", se le saca el resto de la división entera a 11. Se obtiene de esta forma un número (del 0 al 10) (que llamamos "valor 2"). Sacamos la diferencia entre 11 y el "valor 2", y obtenemos un valor comprendido entre 1 y 11 (llamémosle "valor 3").

Si "valor 3"=11, el código verificador es cero. Si "valor 3"=10, el código verificador es 9. En otro caso el dígito verificador será el dígito obtenido


Wiki: Documentación y consigna, para más info



                / ,-\      _ ___
               | (  '\    |-|   |._
        ___     )_ _/     | |   |  |
       [___]   /  `\____  | |   |_.'
       |  ^|  /  \_____/) |-|___|
       |   | /    /   _:::_))_(___
       |   |/'-._/_   |___________|
       '-;_|\_____ `\ ||"""""""""||
         | `######|_|_||         ||
         \ ._  _,'{~-_}|         ||
         _)   (   {-__}|         ||
        /______`\ |_,__)         ||
