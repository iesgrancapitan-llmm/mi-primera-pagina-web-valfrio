## Indica las características propias del lenguaje XML.
Es un lenguaje de marcas creado por la W3C basado en SGML para almacenamiento e intercambio de información estructurada. Lo más característico es que se puede emplear para definir otros lenguajes de marcas (es un metalenguaje).   

Las principales características son: 
- Extensible, se pueden definir nuevas etiquetas
- Verátil, separa contenido, estructura y presentación 
- Estructurado, se puedo doledar datos a cualuiqer nivel de complejidad
- Validable, cada documento se puede validar frente a un DTD
- Abierto, independiente de las empresas y sistemas operativos.
- Sencillo, fácil de aprender y usar.
## Identifica la estructura de un documento XML y sus reglas sintácticas.
La estructura será siempre de árbol, donde hay un nodo raíz, que es la primera marca de la cual cuelgan todo el resto de marcas de un documento, de forma que hay siempre una estructura donde una marca "padre" contiene marcas "hijos" que cuelgan de esta.   

La estructura siempre es: 
- Declaración de XML
- Declaración del DTD
- Cuerpo del documento
- Epílogo


Enumeraré normas sintácticas más básicas.
- las etiquetas son sensibles a las mayusculas y solo algunos carateres pueden usarse para definirlas, como los _
- No puede haber un espacio o salto de linea antes del nombre de una etiqueta (aunque sí por detras).
- Debe haber un nodo raíz siempre.
- Las etiquetas que se abren deben cerrarse siempre.
- Los elementos pueden tener atributos que dan información adicional sobre ellos. 
- Los atributos deben ir entrecomillados, aunque sean arbitrarios.
- Los elementos puede estar vacíos.
- Está formado por etiquetas que abren y cierran de manera seguida

## En XML qué es un nodo raíz
Es la primera marca que abre en un documento XML y que contiene a todo el resto de marcas, por ejemplo: 
```
<libros>
    <libro>
    El guardían entre el centeno
    <libro>
    <libro>El señor de las moscas<libro>
<libros>
```
Podemos ver como ```<libros>``` es el nodo raíz.
## Indica qué es un elemento vacío. Ejemplos
Un elemto vacio es una etiqueta que no contiene valor.   
```<libro genero='romance'/>```   
sería una etiqueta vacia, pues no tiene ningun contenido. 
## Qué sentido tiene crear documentos XML bien formado.
El sentido radica en que el documento sea interpretable por los procesadores sin lugar a ningún tipo de ambigüedad. De esta forma podemos estandarizar las reglas y hacer que los documentos sean fácilmente intercambiables.
## Qué es un espacio de nombres. Ventajas de uso.
Con el fin de que no haya problemas de ambigüedad con los elementos y atributos que pueden coincidir en nombre en diferentes contextos, nace el espacio de nombres.   

De esta forma referenciando el espacio de nombre, una suerte de contexto, podemos distinguir por ejemplo la marca carta en un juego de póker con la carta de un restaurante.   

La URI es el identificador de recursos uniforme. 
## Entidades en XML. Crea un XML con las entidades vistas en clase.
Son formas de escribir caracteres reservados en un documento, de forma que el procesador no los intepretará como su función sino como su carácter ASCII (o UTF). 

[Entidades](Entidades.xml)

## Comentarios en XML. Muestra uno de los ejercicios anteriores con el enunciado dentro de un comentario. Dentro del comentario deben aparecer dos guiones.
[Comentario](Comentario.xml)