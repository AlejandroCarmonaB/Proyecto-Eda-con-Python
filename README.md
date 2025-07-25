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

8-. Comenzamos el analisis descriptivo haciendo un describe para ver las estadisticas generales con la media,maximos,minimos, cuartiles y
vemos un conteo de trabajos para ver cuales son los mas usuales y los que menos.

9-. Se comprueba la proporcion de si y no que tenemos y se hace una tabla de la correlacion entre las variables que tienen entre ellas.

10-.Ahora empezamos a hacer una visualizacion de datos empezando con dos graficas de barras para ver la cantidad de clientes por edad.

11-. Hacemos un diagrama de bigotes y cajas para ver si hay diferencias economicas entre los que contratan y los que no.

12-. Se hace un diagrama de barras con todos los trabajos y si contratan o no, divididos por trabajo. Hacemos esto para comparar los 
trabajos que tienen mayor o menor exito en la campaña.

13-. luego hacemos otro diagrama de cajas para ver lo que influye el tiempo de llamada con la decision de aceptar o rechazar la oferta.

14-. Hacemos un mapa de calor para comprobar la correlacion entre los valores numericos de nuestro dataframe y ver si hay patrones 
fuertes.

## Conclusiones:
Viendo las graficas vemos que la mayoria de clientes se concentran en el rango de edad entre 25 y 45 años, y habria que concentrarse mas 
en estas edades. Sin embargo no habria que dejar de lado a los jubilados y estudiantes, ya que, pese a ser en menor cantidad, suelen 
tener un gran porcentace de exito en contratar algun producto.
Sin embargo sectores o trabajos mas populares tiener menor exito. Tambien el equipo de marquetin deberia de buscar una estrategia cuando 
contactemos con los clientes para que la llamada se alargue lo maximo posible ya que cuanto mas dure, mas posibilidades de que adquiera 
algun producto nuestro habra.
Tambien vemos que no hay mayor o menor indice de contratacion segun sus ingresos, asique no es algo que afecte directamente al cliente.
