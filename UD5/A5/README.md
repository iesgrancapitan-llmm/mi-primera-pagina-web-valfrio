# UD5 A5. Validación. Conceptos

1. **Indica con una X las afirmaciones verdaderas:**

- [ ] Los DTDs son más ricos y poderosos que los XML Schemas

- [ ] Los DTDs están escritos de acuerdo a la sintaxis XML

- [x] XML Schemas soportan tipos de datos

- [x] XML Schemas soportan namespaces
- [ ] XML Schemas tienen el nodo raíz schema con la URL que contiene la definición de todos los elementos y atributos que se pueden utilizar en un esquema. Eso quiere decir que para programar en XML se necesita estar conectado a Internet.
- [x] En XSD, el atributo xmlns crea un espacio de nombres para cada URL referenciada. Así si hubiese dos elementos con el mismo nombre se diferencian claramente.



2. A continuación aparece la declaración de un esquema XSD. Indica los siguientes elementos:

- prólogo. Define la versión del lenguaje XML y el juego de caracteres utilizado

```xml
<?xml version="1.0" encoding="UTF-8"?>
```

- prefijo del espacio de nombres (opcional)

Viene delante de cada elemento, siendo <xs:>

- espacio de nombres XMLSchema

Seria este: 
```xml
xmlns:xs="http://www.w3.org/2001/XMLSchema"
```

El código:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema 
    xmlns:xs="http://www.w3.org/2001/XMLSchema">
		...
<xs:schema />
```
3. A continuación aparece la vinculación de un esquema a un documento XML. Indica (con una X) si está en nuestro sistema de ficheros local o es un esquema público.

- [x] esquema local

- [ ] esquema público
```xml
<factura num="num_fact_1234"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:noNamespaceSchemaLocation="factura.xsd">
	...
</factura>
```

- [ ] esquema local

- [x] esquema público
```xml
<factura num="num_fact_1234"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.miempresa.com/factura.xsd">
...
</factura>	
```
  
4. De los siguientes tipos predefinidos por el espacio de nombres XMLSchema del W3C, marca con una X los numéricos:
- [ ] normalizedString
- [ ] dateTimeStamp
- [ ] language
- [ ] IDREFS
- [ ] dayTimeDuration
- [ ] NMTOKEN
- [ ] NMTOKENS
- [ ] Name
- [ ] NCName
- [ ] ID
- [ ] IDREF
- [ ] ENTITY
- [x] integer
- [ ] yearMonthDuration
- [x] nonPositiveInteger
- [x] negativeInteger
- [x] long
- [x] int
- [x] short
- [x] byte
- [ ] token
- [x] nonNegativeInteger
- [x] unsignedLong
- [x] unsignedInt
- [ ] ENTITIES
- [x] unsignedShort
- [x] unsignedByte
- [x] positiveInteger

5. Adjunta un fichero .xsd con el siguiente diseño:
```xml
<!-- definición de elementos simples -->
<!-- definición de atributos -->
<!-- definición de elementos  complejos -->
<!-- definición de los tipos simples -->
<!-- definición de los tipos complejos -->
<!-- elemento raíz -->
```

[Fcihero](./adjunto.xsd)

6. Con respecto a la validación con XSD indica:
- Un esquema es un documento *XML* al que se le coloca la extensión _xsd_ . Al ser un archivo XML tiene la estructura habitual de todo documento XML con la obligación de que el elemento _raiz_ se llame _schema_ .
- Etiqueta que identifica la raíz de un documento XML Schema: ```<schema> ```
- Etiquetas que identifican las partes de un esquema:
  - Elementos, definidos con etiquetas __element__. Para indicar los elementos permitidos en los documentos que sigan el esquema.
  - Atributos, etiqueta __attribute__.
  - Tipos simples, que permiten definir los tipos simples de datos que podrá utilizar el documento XML. Lo hace la etiqueta __simpleType___ .
  - Tipos complejos, mediante la etiqueta __complexType___
  - Documentación, información utilizable por aplicaciones que manejen los esquemas. Etiquetas ______ y _____.
- Componentes locales y globales en un esquema:
  - En ámbito __global__. Se trata de los elementos del esquema que se coloquen dentro de la etiqueta raíz schema y que no están dentro de ninguna otra. Estos elementos se pueden utilizar en cualquier parte del esquema.
  - En ámbito __local__ . Se trata de elementos definidos dentro de otros elementos. En ese caso se pueden utilizar sólo dentro del elemento en el que están inmersos y no en todo el documento. Es decir si, por ejemplo, si dentro de la definición de un atributo colocamos la definición de un tipo de datos, este tipo de datos sólo se puede utilizar dentro del elemento xs:attribute en el que se encuentra la definición del tipo de datos.
- Dentro de la etiqueta xs:element, indica:
  - atributos obligatorios: use="required"
  - atributos optativos: use="optional"

7. Definición de un elemento vacío en XSD
```
<xs:element name="vacio" type="vacioTipo"/>
<xs:complexType name="vacioTipo"/>
```

De interés
- https://jorgesanchez.net/manuales/xml/xml-validacion.html
- https://www.w3schools.com/xml/el_restriction.asp
- https://lm-xml-apuntes.readthedocs.io/apuntes/40_esquemas_xml.html#tipos-de-elementos
