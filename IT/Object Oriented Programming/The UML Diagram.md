# The UML Diagram
The UML Diagram, or **Unified Modelling Language**, represents one or more classes and their relation. [^1]
An example UML diagram can be seen here:.
```mermaid
classDiagram
	class Nano{
		- name: String
		- height: int
		- weight: int
		+ Nano(name: String, height: int, weight: int)
		+ Nano()
		+ setHeight(height: int): void
		+ setWeight(weight: int): void
		+ setName(name: String): void
		+ getHeight(): int
		+ getWeight(): int
		+ getName(): String
		+ getBMI(): double
		+ toString(): String
	}
```
The first element on the top is the Class name, followed by the attributes and finally by the accessor accompanied by each parameter and relative types of returns and parameters.
Furthermore, in front of each method and attribute, there is a "+" or "-" sign. The *plus* declares the method or attribute as public, while the *minus* declares it as private.
The constructor can be also not defined inside the UML Diagram, the same applies to the getty and setty methods.
Static methods or attributes are marked by being underlined:.
```mermaid
classDiagram
class myClass{
	- myAttribute: int
	- int myStaticAttribute$
	+ myMethod(): void
	+ myStaticMethod()$: void
}
```
Classes can also be connected to each other with a cardinality, which is how many instances can be connected by showing a number next to the arrow head.
Example:.
```mermaid
classDiagram
class A{
	- stuff: id
}
class B{
	- stuffed: String
}
A --o "0..2" B
```
## Abstraction
Abstraction of a method can be marked with one of the following methods:
- `+abstract myMethod(): returntype`
- *+ myMethod(): returntype*
# Enumerations
```mermaid
classDiagram

class Enumeration {
	MYENUMVAL
	MYENUMVAL2

	+ myEnumMethod(): void
}

<<Enumeration>> Enumeration
```

# Inferface
```mermaid
classDiagram

class Iface{
	+ myMethod(): void
}

class IfaceImplem{
	- myAttr: String
}

Iface ..|> IfaceImplem


<<Interface>> Iface
```
# Extending / Implementing
```mermaid
classDiagram

class myClass {
	- attr: int
	+ method(): void
}

class mySubClass {
	- attr2: String
}

mySubClass --|> myClass

```
## Other arrows
```mermaid
classDiagram

class myClass {
	- attr: int
	+ method(): void
}

class myOtherClass {
	- attr: String
}

class arrayList {
	- idk
}

myOtherClass --> myClass : methodsUsedFromMyClass()

myOtherClass ..> myClass : instantiatesSoCallsConstructor()

myClass --o arrayList

myOtherClass ..> arrayList : instantiates

```






[^1]: [[Object Oriented Programming common practices|Common practices in object oriented programming.]] 