Proyect Limpieza y busqueda de hipotesis

Vamos a limpiar un Data_Csv 

Hipotesis
Yo creo que en los años noventa es donde atacaron mśs tiburones contando el siglo XX y el siglo XXI.






['tiburon'](https://github.com/Sergio-Perez/data-cleaning-pandas/tree/master/INPUT/tiburon.jpeg)





Introduccion:
Primero cargamos el archivo "attacks.csv".      




Seguiremos  mirando el archivo y comprobando cuales de las columnas usaremos para realizar nuestra hipótesis.
Limpiaremos esas columnas y las que creamos necesarias de los valores None  y rellenaremos si hiciera falta los valores. Despué de hacer ese recuento de Nones y haber realizado la limpieza. Nos quitamos las columnas duplicadas. Haciendo una comprobacion visual veo que hay varias columnas que son iguales “Case Number” tiene dos columnas que son iguales a ella como “Case Number.1” y “Case Numbaer.2” por lo que me dispongo a eliminarlas. También elimino una de las columans con nombre “href” ya qu tiene otra columna con los mismos valores. Ya que hize una función llamada comparar que miraba si eran iguales. Comprobamos también que “Unnamed: 22" y “Unnamed: 23” son la misma y limpio una de ellas.



Después limpiamos los valores None de las dos columnas principales que vamos a usar “Year” y “Case Number”. Borramos las filas de ellas que contengas Nones.


Voy a crear una nueva columna llamada “Decada” y la voy a crear filtrando los valores de year en cada una de las decadas del siglo XX y siglo XXI . Y lo voy a usar para compara los casos que ocurrieron en esas decadas. Depués elimino los valores 0 que salen en la columna Decada.
Saco un gráfico de esa solución. 
 Y sacar el resultado de si mi hipótesis es verdadero o falso.




Usamos estas librerias:

import matplotlib
import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
import re
