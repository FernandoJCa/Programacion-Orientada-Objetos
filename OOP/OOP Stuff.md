# Brief Introduction 

## Indices

- Cosas a tener en cuenta
- **Background** 
- Y bueno, que es un objeto? 
- Pero bueno, y que es una Clase?
	- Anatomía de una clase (Nombre, Atributos, Métodos, Constructores, entre otros)
- LOS PILARES (JOJO REFERENCE)
  - Encapsulación  
  - Herencia
  - Polimorfismo
  - Composición
- Modelado de Objetos mediante Diagramas
  
**Cosas a tener en cuenta**
 Este material esta altamente influenciado por el libro *The Object-Oriented Thought Process* de Matt Weisfeld. Por lo que **recomiendo altamente** dedicarle una lectura a conciencia de dicho material.
 
 Además, rescato algunas definiciones del gran [Hilo](https://x.com/AngieMatiz6/status/1731398516411441164?s=20) creado por [AngieMatiz6](https://twitter.com/AngieMatiz6)debido a que considero que son muy sencillas de entender. Debo de aclarar que no estarán descritas como tal, pero si ayudaron en gran medida a suavizar las definiciones. 
 
 La idea principal de este material es brindar una pequeña introducción a la POO, desacoplando los conceptos que la rodean de un lenguaje en especifico. De esta manera, buscamos que puedas entenderlos y aplicarlos al lenguaje que desees. 
 
 Tambien debo de avisar que en el libro antes mencionado, el autor trabaja los métodos públicos como *interfaces* que no deben de ser confundidas con las *interfaces* que implementan algunos lenguajes de programación como Java y C#. Para nosotros las *interfaces* serán afectivamente las implementaciones de lenguajes como Java y C#, y no métodos públicos. *(Aunque siendo sincero, no me desagrada la forma como llama a los métodos públicos en un inicio)*
 
 Puedes tomar este material como una traducción o una interpretación.
 
 ***Have fun.***

### Background 

POO es un paradigma de programación basado en el concepto de los *objetos*, los cuales pueden contener datos y Código: Nos referiremos a los datos como atributos y al código como los métodos. 

Pero, que es un paradigma de programación? Y porque nos importa tanto? 

Hasta este punto, has desarrollado ejercicios en un paradigma imperativo, específicamente procedural, donde para llevar acabo la solución haces uso de procedimientos (Funciones).

Ahora POO nos presenta una nueva manera de resolver problemas usando _objetos_ y para ello tenemos que estudiar: Que son, que es una clase, los pilares de POO y muchas otras cosas mas.

Ademas, tengamos en cuenta que POO nos presenta herramientas que nos permitirán modelar **Sistemas del Mundo Real**. 

Nota: Los lenguajes que usas hoy en día como Python, Java, JavaScript, entre otros. Son considerados multiparadigmas ya soportan distintos paradigmas en mayor o menor medida. 

Así que si, la POO no es solo de Java (Viva Java), es algo que se comparte entre todos los lenguajes.

### Y bueno, que es un objeto? 

La pieza fundamental, el cubo, la piedra primigenia. Es el bloque de construcción de un programa OO. Piénsalo de esta manera, una solución que implemente POO no es mas que una colección de objetos que poseen ciertas características que permiten, entre otras muchas cosas, sus relaciones, su identidad. Y hablando de identidad.

**Los atributos**, son las variables de los objetos, solo que aqui se llaman *atributos*. Son los datos que representan el estado de un objeto. 

Además, también podemos entender un objeto por su _Comportamiento_ el cual se ve definido por los **métodos** (Las funciones de toda la vida, solo que aqui se llaman distinto.)

### Pero bueno, y que es una clase?

Corto y al pie, una clase es: Un molde, como el que usas para hacer galletas. 

*Pongámonos en situacion*, quieres hacer galletas, tienes hambre e hiciste masa para galletas, te quedo super rica. Entonces agarras una de estas cosas que tienen forma de galleta (El molde, La Clase) y te ayudan a cortar la masa, ahora quieres comer muchas galletas, por ende haces cinco cortes con el molde que compraste (El que tiene forma de estrella). Esas 5 galletas son tus objetos, los cortes que le hiciste a la masa con tu molde (La clase).

#### Anatomía de una Clase 

##### Nombre
Es esto importante? Si, de esta manera especificas la identidad de la clase. Tiene que ser un buen nombre, ser descriptivo, acompañar el significado y el sentido de una clase. 
##### Atributos
Representan el estado de un Objeto debido a que ellos almacenan la informacion del objeto.
##### Métodos
Estos representan el comportamiento de un objeto.
##### Constructores
Los constructores son algo realmente nuevo para las personas que estan acostumbradas a un paradigma distinto al OO. Un constructor no deja de ser un método especial que permite construir un objeto, estos métodos tienen el mismo nombre que la clase y no retornan nada. 

El compilador es capaz de reconocer este método especial y lo considerara como un *constructor*.

Un constructor es llamado cuando se crea un objeto nuevo, y lo que se encuentra dentro de el es el código necesario para iniciar un nuevo objeto con todos sus atributos. 

### Los pilares

#### Encapsulación

Una de las grandes ventajas de usar objetos, es que un objeto no necesita revelar todos sus atributos y sus comportamientos. En un buen diseño OO (Bueno, lo que es generalmente aceptado como bueno) un objeto solo debería revelar los comportamientos necesarios para que otros objetos puedan interactuar.

La encapsulación nace de la necesidad en el desarrollo de Software de que existe cierta informacion que queremos ocultar y evitar que otras partes del código accedan a el o interactúen con el.
 
De aqui nacen los Getters, Setters. Que básicamente son métodos que controlan el acceso y la asignación de los atributos de un Objeto.
#### Herencia
 **Oh boy, ahora toca algo complicado.**
 
 **Herencia**: Una de las *características* mas importantes de la POO es la reutilización del código. POO te permite definir **relaciones** entre clases para facilitar la reutilización de código, un mejor diseño y una mejor organización de las clases. 
 
 Podemos entender la herencia como la capacidad que tiene una clase de heredar (ceder?) sus atributos y metodos a las clases herederas. En terminos un poco mas sencillos, podemos entender la herencia como una relacion Padre-Hijo donde El Padre hereda a su Hijo ciertos metodos y atributos.
 
 Esto permite la creacion de nuevas clases mediante la abstraccion de los atributos y comportamientos comunes.  

**Superclass y Subclass**: Superclass (Superclase) o clase padre, contiene todos los atributos y comportamientos que son comunes a las clases que lo heredan. 

Por otro lado, Subclass (Subclase) o clase hija, contiene todos los atributos y comportamientos heredados de la clase padre. 

Ahora necesitamos tocar un tema tanto complicado, la **Abstraccion**. Podemos darnos cuenta que la herencia puede llegar a ser un poco complicada a medida que el Arbol Genealogico crece, para evitar este tipo de problemas tenemos que realizar buenas decisiones de diseño previo antes de implementarlo en nuestro problema. **El poder de la herencia recae sobre la abstraccion y las tecnicas de organizacion**

**Herencia Multiple**: La herencia multiple significa en pocas palabras que una clase puede tener muchas clases padres. Ahora, el poder aplicar herencia multiple o no dependerá del lenguaje con el que estemos trabajando.

Lenguajes como Java y C# solo permiten que sus clases tengan una unica clase padre, sin embargo, puedes tener muchas clases hijo. A esto se le conoce como Herencia Unica

C++, por otro lado permite la herencia multiple sin problemas, es decir, permite que una clase hijo tenga muchos padres. 

Antes de salirnos del tema de la Herencia tenemos que hablar de los contratos.

Los contratos, como bien sabemos, es aquello que estamos de acuerdo a cumplir y que no podemos romper. Son en otras palabras, ciertas reglas de juego que comprometemos a cumplir en todo momento y a veces, durante un periodo de tiempo. 

En lenguajes modernos, existen dos formas de implementar contratos.

**Clases Abstractas**: Las clases Abstractas son una de las formas de implementación de contratos. La clase abstracta se define como una clase que contiene uno o mas metodos que pueden poseer una implementacion previa. Y ademas, no puedes instanciarlas. Las clases Abstractas no obligan a la clase que las hereda a implementar todos sus métodos, ya que algunos de ellos pueden ser heredados con una implementación dada por la misma clase abstracta. 

{NOTA: USAR EJEMPLO DE LAS FORMAS DEL LIBRO CAP 8}

**Interfaces**: Antes de entrar en el tema puede que hayas escuchado que C++ no tiene definido interfaces. En este caso, para C++ una clase abstracta cumple las funciones de una interface. 

Entonces, te preguntaras: Si una clase abstracta provee la misma funcionalidad que una interface, por que lenguajes como Java y C# se molestan en implementar interfaces (Teniendo en cuenta que tambien implementan clases abstractas)?

La respuesta radica en la Capacidad de la Herencia en estos lenguajes: C++ posee herencia multiple lo que permite que una clase hijo herede muchas clases padres, que a su vez estas pueden ser clases abstractas. Java y C# no poseen herencia multiple, poseen herencia Unica, aqui en donde entra en accion las interfaces. Java y C# permiten **implementar** mas de una interface, mas no **heredar** mas de una clase. 

Aunque la explicación anterior no explica que es una interface en si, procedemos a explicarlo ahora: Las interfaces son una poderosa forma de implementar contratos, las interfaces no son categorizados como una clase (Abstracta o no). Además, es importante anotar que a diferencia de una clase abstracta los metodos de una interface NO deben de tener una implemetacion. Como resultado, cualquier clase que implemente una interface debera de proveer una implementacion para todos sus metodos.  

Por ejemplo, concretamente en Java, una clase **hereda** de una clase abstracta, mientras que una clase **implementa** una interface. 
#### Polimorfismo

No se cuantas veces he dicho y escuchado esto a lo largo de mi vida como estudiante y dev. Pero, aqui vamos de nuevo. 

Polimorfismo viene de una palabra griega que literalmente significa Muchas Formas (Poli, Muchas; morfe, formas)

Una vez tenemos claro que significa la palabra, veamos su función en la POO.

Si bien polimorfismo es algo que esta estrictamente acoplado con la herencia, es muchas veces citado de manera separada como uno de las mayores ventajas de la POO. En la herencia, todas las subclases heredan los comportamientos de la superclase. Sin embargo, cada subclase puede tener una forma distinta de realizar esos comportamientos.

Dicho de otra manera, todas las subclases heredan los métodos de la superclase. Sin embargo, cada subclase puede implementarlos de maneras distintas si así lo requieren debido a que pueden comportarse de manera distinta a la superclase sin dejar de perder su relación de herencia. 

Y si, aqui veremos la famosa palabra Override.

{VOLVEMOS AL EJEMPLO DEL CAPITULO 8, LETS GOOOO}

En resumen, polimorfismo es la capacidad que tiene una clase de cambiar el comportamiento de un método para ajustarlo a sus necesidades. 

#### Composición
Naturalmente, en algun momento de esta charla llegaste a pensar que un Objeto puede llegar a contener otro Objeto. A esto le llamamos Composición.

Justo como la herencia, la composición provee un mecanismo para construir objetos. 

Cuando construimos relaciones entre objetos podemos pensarlo de distintas maneras. En una herencia consideramos una relación *Es-un/una*, por otro lado, la composición considera la relación como *Tiene-un/una*

Pongamos como ejemplos un Televisor y un Mamífero.

Un televisor *Tiene-una* tarjeta de video, Un televisor *Tiene-una* tarjeta principal.
Pero una tarjeta de video no *es-un* televisor, obviamente. 

Un mamífero *Es-un* gato, un Mamífero *Es-un* Perro. 
De igual manera, un perro *Es-un* mamífero y un gato *Es-un* mamífero.\

{Recurrir al ejemplo del Cap 1, Abstraccion}

**Tipos de composición**:
 - Agregación: Significa que un objeto *Complejo* esta compuesto de otros objetos. Lo observas como un todo, es decir que este objeto complejo no puede vivir sin los objetos que lo componen.
 - Asociación: Significa que un objeto quiere que otro objeto haga algo por el. Eso significa que el primer objeto no necesita del segundo objeto en si, solo lo llama cuando lo considera necesario.
 **Cardinalidad**:
 Suponiendo el caso de una clase Employee, que tiene una relación con las siguientes clases:
 - Division
 - JobDescription
 - Spouse
 - Child

La siguiente tabla ayuda a representar de mejor manera la cardinalidad:

![[cardinalidad.png]]

Donde 0..1 significa que un employee puede tener ninguna o una esposa. 0..n significa que un employee puede tener ningun hijo y un numero ilimitado de hijos. 

Y si, las relaciones de cardinalidad uno-a-muchos se representan como Arrays/Listas dentro del codigo.


---

#### Sigo pensando donde colocar esto



private, permite esconder los atributos y métodos, estos pueden ser accedidos UNICAMENTE por la misma clase
public, permite mostrar los atributos y métodos luego de que se cree un objeto
static, significa que solo existirá una copia de ese atributo o método para todas las instancias de una clase. Además static permite que los atributos y métodos sean llamados sin necesidad de crear un objeto.
