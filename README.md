Training_F1
===========
@author: Victor

Entrenamiento Phyton - Fundamentos

**VERIFICACION DE CUIT/CUIL** (genérico)

El CUIL/CUIT consta de 11 números. Los 10 primeros (2 + 8) constituyen el código de identificación y el último, el dígito de verificación. Para obtener esta verificación se procede de la siguiente forma:

A cada dígito del código, se lo multiplica por los siguientes números (respectivamente) 5, 4, 3, 2, 7, 6, 5, 4, 3, 2 y cada valor obtenido, se suma para obtener una expresión (que llamaremos "valor 1").

A este "valor 1", se le saca el resto de la división entera a 11. Se obtiene de esta forma un número (del 0 al 10) (que llamamos "valor 2"). Sacamos la diferencia entre 11 y el "valor 2", y obtenemos un valor comprendido entre 1 y 11 (llamémosle "valor 3").

Si "valor 3"=11, el código verificador es cero. Si "valor 3"=10, el código verificador es 9. En otro caso el dígito verificador será el dígito obtenido

***

**DIGITO VERIFICADOR DE PATENTES DE AUTOMORES (CABA)**
 
Los dominios o patentes de los automotores están formados por 3 letras y 3 números.
Cada letra tiene una representación numérica. Para determinar la validez del dominio y asegurar su correcto ingreso, se utiliza un algoritmo digito verificador.

De este modo, por ejemplo, el dominio de un automotor podría ser *ALM432*

Tabla de relación letra-número

A 14
B	01
C	00
D	16
E	05
F	20
G	19
H	09
I	24
J	07
K	21
L	08
M	04
N	13
O	25
P	22
Q	18
R	10
S	02
T	06
U	12
V	23
W	11
X	03
Y	15
Z	17


Para determinar el dígito verificador, se toman las letras y se reemplazan por su correspondiente número. 
Para el caso que tomamos, si el dominio es ALM432, el reemplazo dará: 140804432
A partir de esta conversión, se suman los números de derecha a izquierda de forma alternada:

1 4 0 8 0 4 4 3 2  >>> entonces: 2+4+0+0+1 = 7 y 3+4+8+4 = 19

*DV (digito verificador) = 71*

Si en cualquier caso, la suma resultante es un número mayor o igual a 10, se debe sumar hasta obtener un dígito. Para el caso ejemplo 19 se sumará como 1+9 = 10 y 1+0=1, siendo entonces 1 el segundo dígito del dígito verificador resultante.

Otros casos posibles: Es el de los dominios no actualizados como C1661855. Se reemplaza la letra por el número según tabla C1661855 = 001661855
 
Luego, se procede igual a los casos anteriormente mencionados. Se suman los números desde la “derecha” a la “izquierda” alternados 5+8+6+1=20=2+0=2  y 5+1+6=12 = 1+2=3  Entonces el Digito Verificador es 23. Igual que en los casos anteriores, si el dígito obtenido es mayor o igual a 10, se suman sus dígitos (14 pasará a ser 5).


Algunos dominios para validar pueden ser:

SPN725 DV 69
DFN811 DV 41
ETQ290 DV 31
GQX429 DV 64




***
//// endif

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
