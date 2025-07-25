# Proyecto Eda con Python

## Propósito del proyecto
El propósito de este proyecto es averiguar que factores pueden influir en la contratación de un producto lanzado por la entidad bancaria
(ya sea hipoteca, prestamo, etc...) usando datos de campañas y clientes de un banco.

## Pasos para realizar el analisis exploratorio
1-. He cargado el archivo bank y he hechado un primer vistazo para ver filas, columnas, tipo de dato y cantidad de valores nulos. Al cargarlo
me aparecia una columna adicional llamada Unnamed que he eliminado porque no era util ya que era un indice ascendente igual al que ya teniamos.

2-. He modificado el tipo de dato de algunas columnas, ya que estaban como floats y no tiene mucho sentido. Tambien he pasado valores que estaban 
en formato String a tipo numerico, ya que posteriormente es posible que deba operar con ellos. Tambien he quitado todos los valores nulos por 
valores que puedan tener sentido, y, en caso de date, lo he eliminado ya que son muy pocos datos y considero que no pueden influir en gran 
medida si los quito.

3-. Compruebo que ya no hay valores nulos ni duplicados.

4-. Ahora pasamos a cargar el archivo de customers, como es un excel de varias hojas, he de combinarlas para que me pueda aparecer todo el 
conjunto de datos de una. Aqui tambien me aparece la columna Unnnamed que desechamos por los mismos motivos que la anterior. Compruebo 
estructura de los datos,valores,nulos y si hay filas duplicadas.

5-. Procedo a unir las dos tablas para tener un mejor visionado de ambas. Las uno por la columna Id, ya que compruebo que tienen los mismos valores.

6-. Despues de unirlas vuelvo a comprobar que no hayan duplicados, y, muy importante, compruebo fila a fila que los Id coinciden y no son
diferentes.

7-. Una vez unidas las tablas, procedo a eliminar la columna id de mi dataframe, ya que es un dato que para nuestro análisis no aporta 
informacion que pueda ayudar a esclarecer algo.
