# UD1 A1 Lenguajes de marcas

## Contesta a las siguientes preguntas en el README.md de este repositorio. Utiliza el lenguaje Markdown y el editor Visual Studio Code con su plugin correspondiente:

### 1. Indica qué es un lenguaje de marcas. ### 
Es un lenguaje informático que pretende usar etiquetas o marcas para dar información acerca de la estructura del texto o su presentación. Debe ser amigable con el usuario, a la vez que concreto y conciso. También es una serie de comvenciones de marcas para codificar el texto. También debe de especificar: 
   - cúales son las marcas permitidas
   - cúales son las necesarias
   - cómo una marca se distingue del texto
   - cuál es su significado
### 2. Características generales de los lenguajes de marcas.
Debe cumplir con varias condiciones: 
   - Debe estar hecho en **texto plano**, de manera que sea facilmente reconocible por los usuarios. La razón principal es que los archivos de texto plano son compatibles con mucha facilidad entre sistemas operativos o diferentes editores, pues solo son cadenas de binario codificado en UFT-8, ASCII  o similares. También es de igual importancia que una persona podría leerlos a simple vista. 
   - Debe también ser **compacto**, es decir; que las marcas se merjan con el texto de manera que de una sola pasada puedas entender el texto con la formación de formato y estructura. También habla de no tener que usar otro tipo de software par aneterdelo. 
   - Que sea **flexible**, pues cada vez van **especializandose** teniendo apliaciones en más sectores; llegando a mezclarse con otros lenguajes de progrmación y hasta entre distintos lenguajes de marcas.
   - Por último, que sean sencillos de aprender y trabar . En definitiva que sean **amigables con el usuario**.
### 3. Clasifica los lenguajes de marcas e identifica los más relevantes.
   - *De presentación* : Se encargan solamente de darle **formato al texto** sin darle estructura. Un ejemplo puede ser poner el texto en negrita. UN buen ejemplo puede ser **RTF** y **TeX**.
   - *Descriptivo* : Estos se encargan de la otra parte importante del documento, la **estructura**. Un ejemplo de estos son las listas anidadas, que si bien no cambian como se presenta el texto si cambian la estructura de este. El lenguaje mas importante es sin duda **XML** y todos sus derivados (EBML, RDF...)
   - *Híbrido* : posee marcas de ambos lenguajes, siendo usado para **dar formato y estructura**. Un par de ejemplos pueden ser **HTML** y **WML**. 

### 4. Indica los distintos ámbitos de aplicación de los lenguajes de marcas.
   1. *Desarrollo web* : El uso principal es el desarrollo de paginas web estáticas o dinámicas usando HTML.
   2. *Ámbito científico* : La representación de formulas en documentos es muy tedioso, de forma que se diseñó MathML para poder representarlas mucho más fácilmente. 
   3. *Gráficos vectoriales* : Al aumentar el tamaño de imagen de un formato *.jpg* se pierde calidad. Con los gráficos vectoriales no, los cuales están escritos en SVG. 
   4. *Metainformación* : Los datos sobre el mismo documento son lo llamados metadatos (por ejemplo la fecha de creación de este o su autor). Estos datos son claves al filtrar la información. Puede escribirse por ejemplo en HTML. 
   5. *Bases de datos*  : Para una consulta de información muy rápida, muchas bases de datos relacionales permiten transformar la información en un lenguaje de marcas. 
   6. *Intercambio de información* : Al ser tan ligero permite la compartición de grandes cantidades de información de manera sencilla, segura y fiable. 
   7. *Mensajería* : Unas de las principales cualidad que debe tener un servicio de mensajería es que sea sencillo y flexible. Los lenguajes de marcas facilitan mucho los sistemas tradicionales y permiten que sean más facilmente legibles. 
### 5. Inserta un trozo de código de cada uno de los lenguajes de marcas que se indican a continuación. Añadir a cada trozo de código un pequeño resumen sobre su estructura y la aplicación asociada que los procesa:
1. *HTML* :  
```
<html>
	<head>
		<title>Mi página de ejemplo</title>
	</head>
	<body>
	Aquí va el contenido
	</body>
</html>
``````
2. *iCal* : 

```
BEGIN:VCALENDAR
 VERSION:2.0
 CALSCALE:GREGORIAN
 BEGIN:VEVENT
 SUMMARY:Access-A-Ride Pickup
 DTSTART;TZID=America/New_York:20130802T103400
 DTEND;TZID=America/New_York:20130802T110400
 LOCATION:1000 Broadway Ave.\, Brooklyn
 DESCRIPTION: Access-A-Ride to 900 Jay St.\, Brooklyn
 STATUS:CONFIRMED
 SEQUENCE:34
 BEGIN:VALARM
 TRIGGER:-PT10M
 DESCRIPTION:Pickup Reminder
 ACTION:DISPLAY
 END:VALARM
 END:VEVENT
 BEGIN:VEVENT
 SUMMARY:Access-A-Ride Pickup
 DTSTART;TZID=America/New_York:20130802T200000
 DTEND;TZID=America/New_York:20130802T203000
 LOCATION:900 Jay St.\, Brooklyn
 DESCRIPTION: Access-A-Ride to 1000 Broadway Ave.\, Brooklyn
 STATUS:CONFIRMED
 SEQUENCE:3
 END:VEVENT
 END:VCALENDAR 
 ```
 
3. *vCrd* :

``` 
BEGIN:VCARD
VERSION:1.0
N:Gump;Forrest;;Mr.
FN:Forrest Gump
ORG:Bubba Gump Shrimp Co.
TITLE:Shrimp Man
PHOTO;GIF:http://www.example.com/dir_photos/my_photo.gif
TEL;WORK;VOICE:(111) 555-1212
TEL;HOME;VOICE:(404) 555-1212
ADR;WORK;PREF:;;100 Waters Edge;Baytown;LA;30314;United States of estados unidos 
LABEL;WORK;PREF;ENCODING=QUOTED-PRINTABLE;CHARSET=UTF-8:100 Waters Edge=0D=
 =0ABaytown\, LA 30314=0D=0AUnited States of America
ADR;HOME:;;42 Plantation St.;Baytown;LA;30314;United States of America
LABEL;HOME;ENCODING=QUOTED-PRINTABLE;CHARSET=UTF-8:42 Plantation St.=0D=0A=
 Baytown, LA 30314=0D=0AUnited States of America
EMAIL:
REV:20080424T195243Z
END:VCARD 
```
4. *RSS* :
```
<?xml version=”1.0” encoding=”UTF-8”?>
<rss version=”2.0”>
<channel>
     <title>Página</title>
     <link>http://programandoapasitos.blogspot.com</link>
     <description>Tutoriales DAM</description>
     <item>
          <title>RSS</title>
          <link>http://programandoapasitos.blogspot.com/rss</link>
          <description>Tutorial RSS</description>
     </item>
     <item>
          <title>XML</title>
          <link>http://programandoapasitos.blogspot.com/xml</link>
          <description>Tutorial XML</description>
     </item>
</channel>
</rss>
```
5. *KML* :
```<?xml version="1.0" encoding="UTF-8"?>
<kml xmlns="http://www.opengis.net/kml/2.2"> <Placemark>
 <name>Marca de posición simple</name>
 <description>Pegada al suelo. Se coloca de forma inteligente a la altura del relieve subyacente.</description>
 <Point>
 <coordinates>-122.0822035425683,37.42228990140251,0</coordinates>
 </Point>
 </Placemark> </kml>
 ```


De interés:
- [¿QUÉ es un LENGUAJE de MARCAS? [Diccionario del PROGRAMADOR]](https://youtu.be/3CZCV5-HVRg)
- [Generalidades de los lenguajes de marcas y el formato RTF](https://youtu.be/rga8ORhvVNg)
