---
title: element
slug: Web/API/Element
tags:
  - Referencia_DOM_de_Gecko
translation_of: Web/API/Element
---
{{ ApiRef("DOM") }} Este capítulo proporciona una breve explicación para los métodos generales, las propiedades y los eventos disponibles para los elementos HTML y XML en el DOM de Gecko.

Varias especificaciones aplicadas a los elementos:

- [Especificaciones esenciales del DOM](http://www.w3.org/TR/DOM-Level-2-Core/) —describe las interfaces esenciales compartidas por la mayoría de los objetos DOM en los documentos HTML y XML.
- [Especificaciones HTML del DOM](http://www.w3.org/TR/DOM-Level-2-HTML/) —describe las interfaces para objetos en documentos HTML y XHTML construidos con la especificación base.
- [Especificiones de los eventos DOM](http://www.w3.org/TR/DOM-Level-2-Events/) —describe los eventos compartidos por la mayoría de objetos DOM, construidos con las especificaciones y base DOM [Opiniones](http://www.w3.org/TR/DOM-Level-2-Views/).

Los artículos listados aquí amplían lo antedicho e incluyen enlaces a la especificación apropiada del DOM de W3C.

Mientras que estas interfaces son generalmente compartidas por la mayoría de los elementos HTML y XML, hay muchas más especiales para los objetos particulares listados en la especificación HTML del DOM —por ejemplo las interfaces del [elemento tabla de HTML](/es/DOM/table "es/DOM/table") y [elemento formulario de HTML](/es/DOM/form "es/DOM/form").

### Propiedades

| Nombre                                                                                | Descripción                                                                                                                  | Tipo                                                                                                                            | Disponibilidad                                           |
| ------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| [`attributes`](/es/DOM/element.attributes "es/DOM/element.attributes")                | Todos los atributos asociados a un elemento.                                                                                 | [`NamedNodeMap`](/es/DOM/NamedNodeMap "es/DOM/NamedNodeMap")                                                                    | para [todos](/es/DOM "es/DOM")                           |
| [`childNodes`](/es/DOM/element.childNodes "es/DOM/element.childNodes")                | Todos los nodos hijos de un elemento.                                                                                        | [`Listado de nudo`](/es/DOM/NodeList "es/DOM/NodeList")                                                                         | para [todos](/es/DOM "es/DOM")                           |
| [`className`](/es/DOM/element.className "es/DOM/element.className")                   | La clase del elemento.                                                                                                       | [`Secuencia`](/es/Core_JavaScript_1.5_Reference/Global_Objects/String "es/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [HTML](/es/HTML "es/HTML"), [XUL](/es/XUL "es/XUL") |
| [`clientHeight`](/es/DOM/element.clientHeight "es/DOM/element.clientHeight")          | El alto interior del elemento.                                                                                               | [`Número`](/es/Core_JavaScript_1.5_Reference/Global_Objects/Number "es/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`clientWidth`](/es/DOM/element.clientWidth "es/DOM/element.clientWidth")             | El ancho interior del elemento.                                                                                              | [`Número`](/es/Core_JavaScript_1.5_Reference/Global_Objects/Number "es/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`dir`](/es/DOM/element.dir "es/DOM/element.dir")                                     | La direccionalidad del elemento.                                                                                             | [`Secuencia`](/es/Core_JavaScript_1.5_Reference/Global_Objects/String "es/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [HTML](/es/HTML "es/HTML"), [XUL](/es/XUL "es/XUL") |
| [`firstChild`](/es/DOM/element.firstChild "es/DOM/element.firstChild")                | El primer hijo directo del elemento, `null` si no hay.                                                                       | [`Nudo`](/es/DOM/Node "es/DOM/Node")                                                                                            | para [todos](/es/DOM "es/DOM")                           |
| [`id`](/es/DOM/element.id "es/DOM/element.id")                                        | La identificación del elemento.                                                                                              | [`Secuencia`](/es/Core_JavaScript_1.5_Reference/Global_Objects/String "es/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [HTML](/es/HTML "es/HTML"), [XUL](/es/XUL "es/XUL") |
| [`innerHTML`](/es/DOM/element.innerHTML "es/DOM/element.innerHTML")                   | El contenido y el código que hay dentro del elemento.                                                                        | [`Secuencia`](/es/Core_JavaScript_1.5_Reference/Global_Objects/String "es/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [HTML](/es/HTML "es/HTML")                          |
| [`lang`](/es/DOM/element.lang "es/DOM/element.lang")                                  | El lenguaje de los atributos, texto y contenidos del elemento.                                                               | [`Secuencia`](/es/Core_JavaScript_1.5_Reference/Global_Objects/String "es/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [HTML](/es/HTML "es/HTML")                          |
| [`lastChild`](/es/DOM/element.lastChild "es/DOM/element.lastChild")                   | El último hijo directo del elemento, `null` si no hay.                                                                       | [`Node`](/es/DOM/Node "es/DOM/Node")                                                                                            | para [todos](/es/DOM "es/DOM")                           |
| [`localName`](/es/DOM/element.localName "es/DOM/element.localName")                   | La parte local del nombre cualificado del elemento.                                                                          | [`Secuencia`](/es/Core_JavaScript_1.5_Reference/Global_Objects/String "es/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |
| Nombre                                                                                | Descripción                                                                                                                  | Tipo                                                                                                                            | Disponibilidad                                           |
| [`name`](/es/DOM/element.name "es/DOM/element.name")                                  | El nombre del elemento.                                                                                                      | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [HTML](/es/HTML "es/HTML")                          |
| [`namespaceURI`](/es/DOM/element.namespaceURI "es/DOM/element.namespaceURI")          | El URI del espacio de nombre de ese nodo, `null` si no está especificado.                                                    | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |
| [`nextSibling`](/es/DOM/element.nextSibling "es/DOM/element.nextSibling")             | El nodo inmediatamente posterior al primero dado en el árbol, `null` si no hay.                                              | [`Nudo`](/es/DOM/Node "es/DOM/Node")                                                                                            | para [todos](/es/DOM "es/DOM")                           |
| [`nodeName`](/es/DOM/element.nodeName "es/DOM/element.nodeName")                      | El nombre del nodo de ese elemento.                                                                                          | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |
| [`nodeType`](/es/DOM/element.nodeType "es/DOM/element.nodeType")                      | Un número que representa el tipo del nodo. Lo mismo que `1` para los elementos DOM.                                          | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [todos](/es/DOM "es/DOM")                           |
| [`nodeValue`](/es/DOM/element.nodeValue "es/DOM/element.nodeValue")                   | El valor del nodo. Lo mismo que `null` para los elementos DOM.                                                               | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |
| [`offsetHeight`](/es/DOM/element.offsetHeight "es/DOM/element.offsetHeight")          | El alto de un elemento, tal cual está escrito en la composición.                                                             | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`offsetLeft`](/es/DOM/element.offsetLeft "es/DOM/element.offsetLeft")                | La distancia que hay desde el borde izquierdo del elemento al de su `offsetParent`.                                          | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`offsetParent`](/es/DOM/element.offsetParent "es/DOM/element.offsetParent")          | El elemento del cual todos los cálculos de distancia son actualmente computados.                                             | [`Elemento`](/es/DOM/element "es/DOM/element")                                                                                  | para [HTML](/es/HTML "es/HTML")                          |
| [`offsetTop`](/es/DOM/element.offsetTop "es/DOM/element.offsetTop")                   | La distancia desde el borde superior del elemento hasta el de su `offsetParent`.                                             | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`offsetWidth`](/es/DOM/element.offsetWidth "es/DOM/element.offsetWidth")             | El ancho de un elemento, tal cual está escrito en la composición.                                                            | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`ownerDocument`](/es/DOM/element.ownerDocument "es/DOM/element.ownerDocument")       | El documento en el cual está ese nodo, `null` si no hay.                                                                     | [`Documento`](/es/DOM/document "es/DOM/document")                                                                               | para [todos](/es/DOM "es/DOM")                           |
| Nombre                                                                                | Descripción                                                                                                                  | Tipo                                                                                                                            | Disponibilidad                                           |
| [`parentNode`](/es/DOM/element.parentNode "es/DOM/element.parentNode")                | El elemento original(padre) de ese nodo, `null` si no hay dentro del [documento de DOM](/es/DOM/document "es/DOM/document"). | [`Nudo`](/es/DOM/Node "es/DOM/Node")                                                                                            | para [todos](/es/DOM "es/DOM")                           |
| [`prefix`](/es/DOM/element.prefix "es/DOM/element.prefix")                            | El prefijo del espacio de nombre del nodo, `null` si no está especificado.                                                   | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |
| [`previousSibling`](/es/DOM/element.previousSibling "es/DOM/element.previousSibling") | El nodo inmediatamente anterior al primero dado en el árbol , `null` si no hay.                                              | [`Nudo`](/es/DOM/Node "es/DOM/Node")                                                                                            | para [todos](/es/DOM "es/DOM")                           |
| [`scrollHeight`](/es/DOM/element.scrollHeight "es/DOM/element.scrollHeight")          | Muestra la altura de deslizamiento del elemento.                                                                             | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`scrollLeft`](/es/DOM/element.scrollLeft "es/DOM/element.scrollLeft")                | Obtiene/establece el offset de scroll izquierdo de un elemento.                                                              | [`Número`](/es/Core_JavaScript_1.5_Reference/Global_Objects/Number "es/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`scrollTop`](/es/DOM/element.scrollTop "es/DOM/element.scrollTop")                   | Obtiene/establece el offset de scroll superior de un elemento.                                                               | [`Número`](/es/Core_JavaScript_1.5_Reference/Global_Objects/Number "es/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`scrollWidth`](/es/DOM/element.scrollWidth "es/DOM/element.scrollWidth")             | Muestra el ancho de deslizamiento de un elemento.                                                                            | [`Número`](/es/Core_JavaScript_1.5_Reference/Global_Objects/Number "es/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`style`](/Es/DOM/Element.style "Es/DOM/Element.style")                               | Un objeto representando las declaraciones de los atributos de estilo del elemento.                                           | [`Estilo CSS`](/es/DOM/CSSStyleDeclaration "es/DOM/CSSStyleDeclaration")                                                        | para [HTML](/es/HTML "es/HTML"), [XUL](/es/XUL "es/XUL") |
| [`tabIndex`](/es/DOM/element.tabIndex "es/DOM/element.tabIndex")                      | Obtiene/establece la posición del elemento en el órden de tabulación.                                                        | [`Número`](/En/Core_JavaScript_1.5_Reference/Global_Objects/Number "En/Core_JavaScript_1.5_Reference/Global_Objects/Number")    | para [HTML](/es/HTML "es/HTML")                          |
| [`tagName`](/es/DOM/element.tagName "es/DOM/element.tagName")                         | El nombre de la etiqueta para el elemento dado.                                                                              | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |
| [`textContent`](/es/DOM/element.textContent "es/DOM/element.textContent")             | Obtiene/establece los contenidos textuales de un elemento y todos sus descendentes.                                          | [`Secuencia`](/En/Core_JavaScript_1.5_Reference/Global_Objects/String "En/Core_JavaScript_1.5_Reference/Global_Objects/String") | para [todos](/es/DOM "es/DOM")                           |

### Métodos

| Nombre y Descripción                                                                                                                                                           | Devuelve                                                                                                                      | Disponible                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| `addEventListener( type, handler, bubble)` Registra un controlador de evento para un tipo de evento específico en un elemento.                                                 | -                                                                                                                             | [Todos](/es/DOM/event "es/DOM/event")                    |
| `appendChild( appendedNode )` Inserta un nodo así como el último nodo hijo de este elemento.                                                                                   | [Node](/es/DOM/Node "es/DOM/Node")                                                                                            | [Todos](/es/DOM "es/DOM")                                |
| `blur()` Quita el foco del teclado del elemento actual.                                                                                                                        | -                                                                                                                             | para [HTML](/es/HTML "es/HTML"), [XUL](/es/XUL "es/XUL") |
| `click()` Simula un clic sobre el elemento actual.                                                                                                                             | -                                                                                                                             | para [HTML](/es/HTML "es/HTML"), [XUL](/es/XUL "es/XUL") |
| `cloneNode( deep)` Hace copia de un nudo, y opcionalmente, de todo sus contenidos                                                                                              | [Node](/es/DOM/Node "es/DOM/Node")                                                                                            | para [Todos](/es/DOM "es/DOM")                           |
| `dispatchEvent( event )` Envía un evento a este nodo en el DOM.                                                                                                                | [Boolean](/es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean "es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean") | [Todos](/es/DOM "es/DOM")                                |
| `getAttribute( name )` Devuelve el valor de un atributo nombrado desde el nodo actual.                                                                                         | [Object](/es/Core_JavaScript_1.5_Reference/Global_Objects/Object "es/Core_JavaScript_1.5_Reference/Global_Objects/Object")    | [Todos](/es/DOM "es/DOM")                                |
| `getAttributeNS( namespace, name )` Devuelve el valor del atributo con el nombre especificado, desde el nodo actual.                                                           | [Object](/es/Core_JavaScript_1.5_Reference/Global_Objects/Object "es/Core_JavaScript_1.5_Reference/Global_Objects/Object")    | [Todos](/es/DOM "es/DOM")                                |
| `getAttributeNode( name )` Devuelve la representación del nodo del atributo nombrado desde el nodo actual.                                                                     | [Attr](/es/DOM/Attr "es/DOM/Attr")                                                                                            | [Todos](/es/DOM "es/DOM")                                |
| `getAttributeNodeNS( namespace, name )` Devuelve la representación del nodo del atributo con el nombre especificado, desde el nodo actual.                                     | [Attr](/es/DOM/Attr "es/DOM/Attr")                                                                                            | [Todos](/es/DOM "es/DOM")                                |
| Nombre y Descripción                                                                                                                                                           | Devuelve                                                                                                                      | Disponibilidad                                           |
| `getElementsByTagName( name )` Devuelve un conjunto de todos los elementos descendentes, de un nombre de etiqueta particular, desde el elemento actual.                        | [NodeSet](/es/DOM/NodeSet "es/DOM/NodeSet")                                                                                   | [Todos](/es/DOM "es/DOM")                                |
| `getElementsByTagNameNS( namespace, name )` Devuelve un conjunto de todos los elementos descendentes, de un nombre de etiqueta y espacio particular, desde el elemento actual. | [NodeSet](/es/DOM/NodeSet "es/DOM/NodeSet")                                                                                   | [Todos](/es/DOM "es/DOM")                                |
| `hasAttribute( name )` Verifica si el elemento tiene el atributo especificado o no.                                                                                            | [Boolean](/es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean "es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean") | [Todos](/es/DOM "es/DOM")                                |
| `hasAttributeNS( namespace, name )` Verifica si el elemento tiene el atributo especificado, en el nombre de espacio especificado o no.                                         | [Boolean](/es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean "es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean") | [Todos](/es/DOM "es/DOM")                                |
| `hasAttributes()` Verifica si el elemento tiene o no algún atributo.                                                                                                           | [Boolean](/es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean "es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean") | [Todos](/es/DOM "es/DOM")                                |
| `hasChildNodes()` Verifica si el elemento tiene nodos hijos o no.                                                                                                              | [Boolean](/es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean "es/Core_JavaScript_1.5_Reference/Global_Objects/Boolean") | [Todos](/es/DOM "es/DOM")                                |
| `insertBefore( insertedNode, adjacentNode )` Inserta el primer nodo antes que el segundo, Nodo hijo en el DOM.                                                                 | [Node](/es/DOM/Node "es/DOM/Node")                                                                                            | [Todos](/es/DOM "es/DOM")                                |
| `normalize()` Limpia todos los nodos de texto debajo de este elemento (une lo adyacente, quita lo vacío).                                                                      | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |
| `removeAttribute( name )` Quita el atributo nombrado desde el nodo actual.                                                                                                     | -                                                                                                                             | [All](/es/DOM "es/DOM")                                  |
| `removeAttributeNS( namespace, name )` Quita el atributo con el nombre y nombre de espacio especificado desde el nodo actual.                                                  | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |
| Nombre y Descripción                                                                                                                                                           | Devuelve                                                                                                                      | Disponibilidad                                           |
| `removeAttributeNode( name )` Quita la representación del nodo del atributo nombrado desde el nodo actual.                                                                     | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |
| `removeChild( removedNode )` Quita el nodo hijo desde el elemento actual.                                                                                                      | [Node](/es/DOM/Node "es/DOM/Node")                                                                                            | [Todos](/es/DOM "es/DOM")                                |
| `removeEventListener( type, handler )` Quita un oyente de evento desde el elemento.                                                                                            | -                                                                                                                             | [Todos](/es/DOM/event "es/DOM/event")                    |
| `replaceChild( insertedNode, replacedNode )` Reemplaza un nodo hijo en el elemento actual con otro.                                                                            | [Node](/es/DOM/Node "es/DOM/Node")                                                                                            | [Todos](/es/DOM "es/DOM")                                |
| `scrollIntoView( alignWithTop )` Recorre la página hasta que el elemento se obtiene en la vista.                                                                               | -                                                                                                                             | [HTML](/es/HTML "es/HTML")                               |
| `setAttribute( name, value )` Establece el valor de un atributo nombrado desde el nodo actual.                                                                                 | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |
| `setAttributeNS( namespace, name, value )` Establece el valor del atributo con el nombre y nombre de espacio especificado desde el nodo actual.                                | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |
| `setAttributeNode( name, attrNode )` Establece la representación del nodo del atributo nombrado desde el nodo actual.                                                          | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |
| `setAttributeNodeNS( namespace, name, attrNode )` Establece la representación del nodo del atributo con el nombre y nombre de espacio especificado desde el nodo actual.       | -                                                                                                                             | [Todos](/es/DOM "es/DOM")                                |

### Eventos

Son propiedades correspondientes a los atributos del evento "on" en HTML.

A diferencia de los atributos correspondientes, los valores de esas propiedades son funciones (o cualquier otro objeto trabajando con la interfaz [EventListener](http://www.w3.org/TR/DOM-Level-2-Events/events.html#Events-EventListener)) más bien que una cadena de carácteres. En efecto, asignar un atributo de evento en HTML crea una función envolvente alrededor del código especificado. Por ejemplo, el siguiente HTML:

    <div onclick="foo();">clic aquí!</div>

Si `element` es una referencia a esta `div`, el valor de `element.onclick` será:

    function onclick(event) {
       foo();
    }

El objeto [event](/es/DOM/event "es/DOM/event") es pasado al parámetro `event` de esta función envolvente.

- [onblur](/es/DOM/element.onblur "es/DOM/element.onblur") - (al quitar el foco)
  - : Devuelve el código de manejo de evento para el evento `blur`.

<!---->

- [onchange](/es/DOM/element.onchange "es/DOM/element.onchange") - (al modificar)
  - : Devuelve el código de manejo de evento para el evento `change`.

<!---->

- [onclick](/es/DOM/element.onclick "es/DOM/element.onclick") - (al hacer clic)
  - : Devuelve el código de manejo de evento para el evento `onclick`.

<!---->

- [ondblclick](/es/DOM/element.ondblclick "es/DOM/element.ondblclick") - (al hacer doble clic)
  - : Devuelve el código de manejo de evento para el evento `ondblclick`.

<!---->

- [onfocus](/es/DOM/element.onfocus "es/DOM/element.onfocus") - (al poner el foco)
  - : Devuelve el código de manejo de evento para el evento `onfocus`.

<!---->

- [onkeydown](/es/DOM/element.onkeydown "es/DOM/element.onkeydown") - (al tener una tecla apretada)
  - : Devuelve el código de manejo de evento para el evento `onkeydown`.

<!---->

- [onkeypress](/es/DOM/element.onkeypress "es/DOM/element.onkeypress") - (al apretar una tecla)
  - : Devuelve el código de manejo de evento para el evento `onkeypress`.

<!---->

- [onkeyup](/es/DOM/element.onkeyup "es/DOM/element.onkeyup") - (al soltar una tecla)
  - : Devuelve el código de manejo de evento para el evento `onkeyup`.

<!---->

- [onmousedown](/es/DOM/element.onmousedown "es/DOM/element.onmousedown") - (al tener el botón del ratón apretado)
  - : Devuelve el código de manejo de evento para el evento `onmousedown`.

<!---->

- [onmousemove](/es/DOM/element.onmousemove "es/DOM/element.onmousemove") - (al mover el ratón)
  - : Devuelve el código de manejo de evento para el evento `onmousemove`.

<!---->

- [onmouseout](/es/DOM/element.onmouseout "es/DOM/element.onmouseout") - (al quitar el puntero del ratón)
  - : Devuelve el código de manejo de evento para el evento `onmouseout`.

<!---->

- [onmouseover](/es/DOM/element.onmouseover "es/DOM/element.onmouseover") - (al pasar el ratón encima)
  - : Devuelve el código de manejo de evento para el evento `onmouseover`.

<!---->

- [onmouseup](/es/DOM/element.onmouseup "es/DOM/element.onmouseup") - (al soltar el botón del ratón)
  - : Devuelve el código de manejo de evento para el evento `onmouseup`.

<!---->

- [onresize](/es/DOM/element.onresize "es/DOM/element.onresize") - (al re-dimensionar la pantalla)
  - : Devuelve el código de manejo de evento para el evento `onresize`.