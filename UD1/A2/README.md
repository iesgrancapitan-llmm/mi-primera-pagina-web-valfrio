# A2. Lenguajes de marcas (2ª parte)
## Indica la evolución de los lenguajes de marcas.
### El origen: GML
Los documentos electrónicos tenian falta de compatibilidad entre apliaciones, de forma que la transmisión de estos era imposible. Por ello, y por la falta de herramientas para separar estructura y formato, se creo **GML**.  

IBM creo **GML** (*Generalized Markup Language*) que independizo el documento del dispositivo usando marcas genéricas, a la vez que introdujo marcas para dar estructura al texto.
### La estandarización: SGML
Dada la popularidad de GML se vio la necesiadad de estandarizarlo, dando pie a la creación por parte de ISO del **SGML**.  

Este ya incluye normas de utilización de las marcas, así como que etiquetas están permitidas y donde ubicarlas (todo esto es llamado sintaxis). El DTD especificaba la santaxis según el tipo de documento. Esto hizo que SMGL fuera el padre de mucho de los LM.  

El punto negativo de este es que es muy difícil de aprender debido a su gran potencia. 
### La popularización: HTML
**HTML** nace como la necesidad de que **SGML fuera accesible** para competir contra los editores WYSIWYG. Es muy sencillo de aprender y utilizar sin conocimientos infórmaticos apenas.  

Esto hizo que se produjera mucha cantidad de documentos mal estructurados sobre los años 90. Además la falta de respeto por los estándares agravó la situación. 
### La madurez: XML
Para solucionar los problemas del HTML nace XML, un lenguaje que permite crear etiquetas según tus necesidades. Esto da muchas posibilidades, aunque sigue siendo estricto en que se puede hacer. Cualquier documento debe de ser válido y estar bien formado. 

Es un derivado compatible com SGML, de forma que muchos documentos son fácilmente convertibles. XML es mucho más sencillo que SGML, haciendo que sea mucho más fácil de aprender, a la vez que más flexible. 
## Los lenguajes de marcas son claves para el intercambio de información. Indica las ventajas e inconvenientes.
### Ventajas
- *Sencillez* : con mínimo conocimiento puedes empezar a desarrollar documentos. 
- *Estructurado* : su forma de organizar el documento es clara y de fácil compresión. 
- *Herramientas específicas* : se pueden generar documentos con herramientas que podría usar un usuario sin conocimientos específicos. 
- *Pocos recursos* : ocupan poco espacio y son facilmente transmitibles
- *Despliegue rápido*: es muy rápido generar documentos.
- *Fácil aprendizaje*: no necesitas conocimientos de otras áreas para generar documentos electrónicos. 
- *Estándar* :todos los navegadores y muchas apliaciones usan documentos generados por lenguajes de marcas, lo que hace más fácil el intercambio de información.  

En resumen, son muy sencillos de utilizar, de aprender, comprender y muy aceptados en la comunidad. 

### Desventajas
- *Lenguaje estático* : los cambios requieren de una nueva generación y distribución del documento. 
- *Falta de homogeneidad en la presentación* : como cada navegador interpreta las marcas puede ser distinto. 
- *Información irrelevante* : guarda muchas marcas que pueden convertirse en basura y esto dificulta su correción.
- *Diseño lento* : hay que diseñar su estructura antes de poder generar un documento. 
- *Estiquetas limitadas* : no tiene la misma potencia que otro tipo de documentos.  

En resumen, el documento generado puede tener ciertos problemas a la hora de sufrir cambios o al ser visualizado en diferentes navegadores, asi como el hecho de que generar el documento tiene partes tediosas como generar la estructura o que las mismas marcas dificulten su correción; pero me parece que tienen muchas mas ventajas que incovenientes. 
## Organismos y estándares: W3C y WHATWG
La primera organización que nace para el desarrollo completo de la web fue el **W3C** (*World Wide Web Consortium*), fundando por el creador de la *world wide net*, Tim Berners-Lee. Este nace para crear una comunidad que contribuya a que existan unos estándares que aseguren el correcto desarrollo de la Web.  

Para entender el rol del W3C hay que entender primero que son los estándares: estos son normas que sirven de guía en el desarrollo de tecnología para que funcionen aun siendo desarrolladas independientemente, de manera que deben ser compatibles entre sí.  

Por último los desarrolladores de navegadores web crearon una organización que también desarrolara estandarés para la Web, la **WHATWG** (*Web Hypertext Application Technology Working Group*). Estos se encargan de desarrollar principalmente HTML, DOM y algunas APIs. La W3C de CSS y otras varias tecnologías.  
