## Design Patterns 

### Static vs Dynamic typing 
1. Both related to type checks 
2. Static: 
		- Type checking before run-time and type remains same during lifetime
		- Because type is checked before run-time, how compiler will know the type ? There is no way to guess the type, so need to explicity declare the type of variable.
3. Dynamic
		- Type checking at run-time & type of object can be changed
		- No need to explicit type declaration, while execution seeing the data hold by object, interpreter makes a guess about the type.

### Program to interface not to implementations
1. Basics
	- There are 4 parties: Client code, interface, Developer, Factory
	- Developer
		- It will provide different functionalities
	- Client Code
		- Here we want to make use of functionalities by Developer
		- But we want the client code to clean and flexible.
	- Interface
		- Kind of contract, where we list what functions exactly 'Developer' will provide
	- Factory
		- This will give objects to client code, based on some condition.

2. Flow
	- Now Developer build 2 different classes which implements the interface i.e follow the contract i.e expose the functions mentioned in the contract/interface
	- Then according to some condition, factory will provide the object of a particular class(out of 2 classes developed by the developer) to the client code. 
	- Then client code will call the functions. 

3. Static vs Dynamic typed
	- In static typed languages like java, when factory will provide the object, it must be caught in some variable and the variable must have some type. Now the object could be of any class developed by Developer, but we want to put them in a variable of a particular type. 
		- Therefore in static type languages we have concept of interface, when both those classes of developer implements the interface, their object can be put in the variable of type 'interface'. 
	- In dynamic typed like python, we don't have to specify the type of variable where we are going to put the object returned by the factory. So there is no need of interface construct here, Factory can return object of any class, that will be put in a variable and client code will call the functions using this variable. 
		- Just need to be carefull that class must have all the functions which client code is expecting.
		- Dynamic type language will not throw any error if didn't define some of the functionalities. But this could through an error on runtime, when client code will call the particular function. 
		- Static typed are better in this sense, they maintain a record of which functions all the implementing classes have to provide. 