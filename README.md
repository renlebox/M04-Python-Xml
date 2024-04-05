# M04-Python-Xml
Recursos de python y xml

## XML (Extensible Markup Language):
### Definición simple:
XML es un tipo de archivo que se usa para almacenar datos en un formato estructurado. Piensa en él como un documento de texto que organiza la información de manera que las computadoras puedan entenderla fácilmente.
#### Ejemplo: 
Es como hacer una lista con etiquetas para diferentes partes de un libro, como el título, el autor y los capítulos.
#### Enlace al w3school:
[Aquí](https://www.w3schools.com/xml/) 

## Conceptos clave:
#### Sintaxis XML:
Debes comprender la sintaxis básica de XML, incluyendo etiquetas, atributos y elementos.
#### Document Object Model (DOM):
Conocer cómo se representa un documento XML como un árbol de nodos, lo que facilita la navegación y manipulación del contenido.
#### Event-based parsing: 
Algunos parsers XML funcionan de manera "basada en eventos", lo que significa que desencadenan acciones a medida que encuentran elementos en el documento XML, en lugar de cargar todo el documento en la memoria de una vez.

#### Librerías XML en Python:
En Python, hay varias bibliotecas y herramientas para trabajar con XML, como xml.dom, xml.etree.ElementTree y lxml.
```python
- Codigo xml
<datos>
    <persona>
        <nombre>John</nombre>
        <apellido>Doe</apellido>
        <edad>30</edad>
    </persona>
    <persona>
        <nombre>Jane</nombre>
        <apellido>Smith</apellido>
        <edad>25</edad>
    </persona>
</datos>
```
```
- Codigo python 
import xml.etree.ElementTree as ET

# Parsear el archivo XML
tree = ET.parse('datos.xml')
root = tree.getroot()

# Iterar sobre los elementos persona
for persona in root.findall('persona'):
    nombre = persona.find('nombre').text
    apellido = persona.find('apellido').text
    edad = persona.find('edad').text
    print(f"Nombre: {nombre}, Apellido: {apellido}, Edad: {edad}")
```
#### Métodos de parseo:
Conocer cómo usar estas bibliotecas para analizar documentos XML y acceder a su contenido.
#### Manipulación de nodos: 
Saber cómo agregar, modificar y eliminar nodos en un documento XML utilizando las funciones proporcionadas por estas bibliotecas.
#### Serialización:
Entender cómo guardar los cambios realizados en un documento XML de vuelta a un archivo.

#### Validación XML:
La validación XML es el proceso de comprobar si un documento XML cumple con un conjunto de reglas definidas en un esquema XML (DTD, XML Schema).
DTD y XML Schema: Conocer los diferentes tipos de esquemas XML y cómo se utilizan para definir la estructura y los tipos de datos permitidos en un documento XML.
Herramientas de validación: Familiarizarse con las herramientas que pueden validar documentos XML contra un esquema, como xmllint para DTD o lxml para XML Schema en Python.

## DOM (Document Object Model):
### Definición simple:
DOM es una manera de representar documentos XML como una estructura de árbol en la memoria de una computadora. Cada parte del documento XML se convierte en un "nodo" en este árbol, y puedes acceder y manipular estos nodos fácilmente.
#### Ejemplo:
Imagina un árbol genealógico donde puedes seguir ramas para encontrar a ciertas personas y cambiar sus nombres si es necesario.
#### Enlace al w3school:
[Aquí](https://www.w3schools.com/whatis/whatis_htmldom.asp)

## Conceptos clave:
#### Nodos:
Los elementos individuales de un documento XML, como etiquetas, texto y atributos, se convierten en nodos en el árbol DOM.
#### Padres e hijos:
Los nodos en el DOM tienen relaciones jerárquicas, donde un nodo puede ser el padre, hijo o hermano de otro nodo.
##### Interfaz de programación:
El DOM proporciona una interfaz de programación que te permite acceder y manipular los nodos de un documento XML usando código.

#### Python y DOM:
Conceptos clave:
Módulo xml.dom: Es el módulo de Python que proporciona las herramientas para trabajar con el DOM.
Parseo de documentos: Puedes usar xml.dom.minidom para analizar un documento XML y cargarlo en la memoria como un objeto DOM.
Manipulación de nodos: Una vez que has cargado un documento XML en un objeto DOM, puedes navegar por su estructura de nodos y realizar cambios según sea necesario.
Serialización: Después de realizar cambios en un documento XML a través del DOM en Python, puedes guardar los cambios de vuelta a un archivo XML.
Herramientas útiles:
Métodos de navegación: Aprender los métodos proporcionados por xml.dom para acceder y manipular nodos, como getElementsByTagName() para obtener todos los nodos con una etiqueta específica.
Manejo de excepciones: Al trabajar con el DOM en Python, es importante estar familiarizado con el manejo de excepciones para capturar y manejar posibles errores durante la manipulación del documento XML.

## Python:
## Definición simple: 
Python es un lenguaje de programación que te permite escribir instrucciones para que una computadora las siga. Es conocido por ser fácil de entender y escribir, incluso para quienes no son expertos en programación.
### Ejemplo:
Piensa en Python como un conjunto de instrucciones que le das a una máquina para que haga ciertas tareas, como ordenar una lista de números de menor a mayor.
#### Enlace al w3school:
[Aquí](https://www.w3schools.com/python/)

### Conceptos clave:
#### Sintaxis clara:
Python se destaca por su sintaxis clara y legible, lo que lo hace fácil de aprender y comprender para principiantes y expertos por igual.
#### Biblioteca estándar:
Python viene con una amplia biblioteca estándar que incluye módulos y herramientas para realizar diversas tareas, desde manipulación de archivos hasta creación de interfaces gráficas de usuario.
#### Interpretado:
Python es un lenguaje interpretado, lo que significa que el código se ejecuta línea por línea por un intérprete, lo que facilita la depuración y la experimentación.
#### Multiparadigma:
Python admite múltiples paradigmas de programación, incluyendo programación orientada a objetos, programación funcional y programación imperativa.
### Python y XML:

### Herramientas útiles:
##### Documentación oficial: 
La documentación oficial de Python y sus bibliotecas proporciona recursos útiles y ejemplos para aprender a trabajar con XML en Python.
##### Comunidad y foros: 
La comunidad de Python es activa y ofrece una amplia gama de recursos, incluyendo foros de ayuda donde puedes hacer preguntas y obtener asistencia sobre cómo manejar XML en Python.
