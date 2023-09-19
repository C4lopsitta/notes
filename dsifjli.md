```mermaid
classDiagram
class Car{
	- licensePlate: String
	- name: String
	- registrationNumber: Integer
	- lastRegistrationNumber: Integer$
	+ Car()$
	+ Car(name: String, licensePlate: String)$
	+ getLicensePlate(): String
	+ getLastRegistrationNumber(): Integer$
	+ getName(): String
	+ getRegistrationNumber(): Integer
	+ setLicensePlate(licensePlate: String): void
	+ setName(name: String): void
	+ toString(): String
}
```
