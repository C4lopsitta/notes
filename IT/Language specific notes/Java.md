# Classes
```Java
<visibility> class Name {

	public Name(){} //constructor
}
```

Constructors are a special method that is a Class Method and you usually find two of them:
1. Default constructor (shown in example) with no parameters
2. Attribute constructor, that asks for every attribute when called to make an already filled attributes.
   ```java
   public Name(type param1, type param2) {
	   this.param1 = param1;
	   this.param2 = param2;
   }
```


```mermaid
classDiagram
class Pavimento{
	- id: int
	- name: String
	- material: String
	+ Pavimento()
	+ Pavimento(id: int, name: String, material: String)
	+ getId(): int
	+ getName(): String
	+ getMaterial(): String
	+ setId(id: int): void
	+ setName(name: String): void
	+ setMaterial(material: String): void
	+ toString(): String
}
```
