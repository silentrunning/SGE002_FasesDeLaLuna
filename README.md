# FasesDeLaLuna

Un método simplificado para saber la fase lunar de un día cualquiera puede ser el expuesto en la
dirección **http://mizar.blogalia.com/historias/21732** que dice:
¿cuál fué la fase lunar el día 6 de Diciembre de 2004?

* En primer lugar, sumamos las cifras del año actual ( 2004=2+0+0+4=6 )
* Multiplicamos el resultado por 11: ( 6x11=66 )
* A la cifra anterior, le sumamos la cifra correspondiente al día y la cifra correspondiente al mes que nos interesan: ( 66+6+12=84 )
* Al resultado le restamos 30 sucesivamente hasta que no se puedan seguir realizando sustracciones: ( 84-30=54 ; 54-30=24 - ya no podemos seguir )
* Este resultado es la edad de la Luna el día buscado
  
Así pues el día 6 de diciembre la edad de la Luna es de 24 días, lo cual corresponde a 3 días después del
cuarto menguante. Si el resultado es 0 tendremos luna nueva, si es 7 cuarto creciente, para 14 tenemos
luna llena, para 21 cuarto menguante. Los resultados intermedios determinan los valores entre fases
correspondientes.

El método es válido desde el año 2000 al 2009.

¿Y qué pasa a partir del 2010?

Hay una forma simple de prolongar la validez del método hasta 2019, para ello basta con tratar los dos
últimos dígitos del año como un sólo número, en lugar de cifras individuales, así la suma para el año
2015 sería: 2 + 0 + 15 = 17.

Lo mejor del método es que puede ser válido para cualquier fecha si utilizamos el ciclo metónico que
indica que la misma fase lunar se vuelve a producir en la misma fecha cada 19 años. por tanto si
quieres calcular la fase en una fecha anterior al 2000, puedes sumar 19 repetidas veces hasta que
llegues a una fecha incluida en el rango 2000-2019, para años posteriores basta con restar 19 hasta
encontrarse en el intervalo indicado.


Con estas indicaciones se desea añadir a la clase Date los siguientes métodos:

**moonAge**     indicará la edad de la luna en la forma que se comenta en el blog para la
            fecha contenida en la instancia.
            
**isFullMoon**  indica si en la fecha contenida en la instancia hay luna llena

**isNewMoon** indica si en la fecha contenida en la instancia hay luna nueva

**isFirstQuarter**  indica si en la fecha de la instancia hay cuarto creciente 

**isLastQuarter** indica si en la fecha de la instancia hay cuarto menguante

**fullMoonDay** devuelve el día del mes contenido en la instancia en que hay luna llena

**newMoonDay**  devuelve el día del mes contenido en la instancia en que hay luna nueva

**easterSundayDay** devuelve la fecha del domingo de resurrección del año que se pase como
argumento


En http://blog.cardila.com/2007/04/02/como-calcular-la-fecha-de-la-semana-santa/ dice:
La Iglesia Católica quiso ya desde un principio, conmemorar la muerte de Jesús el mismo día que lo
relatan los evangelios. Ha sido tradición en los judíos celebrar su pascua sirviéndose del calendario
lunar; por supuesto en la época de Jesús, la pascua se regía por los ciclos de la luna. Partiendo de esto,
el calendario de Semana Santa, se obtiene a partir del día de la Resurrección, que es el domingo
siguiente a la luna llena del mes de Nissan (el mes de los judíos) que corresponde a los días entre el 22
de marzo y el 25 de abril. Dicho de otra manera, este día es el domingo después de la primera luna
llena de primavera (la primavera, por lo general, comienza el 21 de marzo).


Los métodos expuestos solo devolverán valores si la fecha de la instancia es posterior al 1 de Enero de
2000. Con otras fechas devolverán un error en tiempo de ejecución con un mensaje de “este método
solo se puede invocar con fechas posteriores al año 2000”
Crear un archivo moonTools.js en la que guardar todas estas definiciones de métodos y subir.
