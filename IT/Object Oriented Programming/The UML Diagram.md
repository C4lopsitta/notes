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

[^1]: [[Object Oriented Programming common practices|Common practices in object oriented programming.]] 