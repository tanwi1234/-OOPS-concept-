

<h1 text-align=center>OBJECT ORIENTED PROGRAMMING</h1>
The main aim of OOP is to bind together the data and the functions that operate on them so that no other part of the code can access this data except that function.
Object-oriented programming aims to implement real-world entities like inheritance, hiding, polymorphism, etc in programming.
Characteristics of an Object Oriented Programming language:

Class: Class in C++ is a blue-print representing a group of objects which shares some common properties and behaviours.
•	A Class is a user-defined data-type which has data members and member functions which can be accessed and used by creating an instance of that class. 
•	Data members are the data variables and member functions are the functions used to manipulate these variables and together these data members and member functions define the properties and behaviour of the objects in a Class.
•	Member functions are method to access data memebers

Objects:- An Object is an identifiable entity with some characteristics and behaviour. An Object is an instance of a Class
 When a class is defined, no memory is allocated but when it is instantiated (i.e. an object is created) memory is allocated.
 Access Modifier: Access Modifiers or Access Specifiers in a class are used to assign the accessibility to the class members. That is, it sets some restrictions on the class members not to get directly accessed by the outside functions.
   3 types of access modifier:
•	Public : The data members and member functions declared as public can be accessed by other classes and functions too
•	Protected: They are not allowed to be accessed directly by any object or function outside the class.  can be accessed only by the member functions inside the class
•	Private : similar to private access modifier the difference is that the class members declared as Protected can be accessed by any subclass(derived class) of that class as well. 
            by default the access modifier for the members will be Private.
*Only the member functions or the friend functions are allowed to access the private data members of a class.
 <b>Friend Class</b>
     A friend class can access private and protected members of other class in which it is declared as friend.

<b>Friend function</b>:  
•	Friends should be used only for limited purpose. too many functions or external classes are declared as friends of a class with protected or private data,
•	it lessens the value of encapsulation of separate classes in object-oriented programming
•	 A friend function can be: 
a) A member of another class 
b) A global function 

*Friendship is not mutual. If class A is a friend of B, then B doesn’t become a friend of A automatically

Polymorphism:-
•	polymorphism as the ability of a message to be displayed in more than one form.
•	Polymorphism is extensively used in implementing inheritance

An operation may exhibit different behaviours in different instances. The behaviour depends upon the types of data used in the operation.
C++ supports operator overloading and function overloading.
•	Operator Overloading: The process of making an operator to exhibit different behaviours in different instances is known as operator overloading.
•	Function Overloading: Function overloading is using a single function name to perform different types of tasks..


Compile time polymorphism: This type of polymorphism is achieved by function overloading or operator overloading.

1.function overloading: When there are multiple functions with same name but different parameters then these functions are said to be overloaded

2.Operator overloading: C++ has the ability to provide the operators with a special meaning for a data type, this ability is known as operator overloading.
•	Almost all operators can be overloaded except few. Following is the  list of operators that cannot be overloaded.
•	. (dot) 
•	:: 
•	?: 
•	sizeof 

Runtime polymorphism: This type of polymorphism is achieved by Function Overriding.
•	Function overriding :when a derived class has a definition for one of the member functions of the base class. That base function is said to be overridden.


Abstraction:- 
•	Data abstraction refers to providing only essential information about the data to the outside world, hiding the background details or implementation.
•	Abstraction using Classes: The class helps us to group data members and member functions using available access specifiers. A Class can decide which data member will be visible to the outside world and which is not.
•	Abstraction in Header files: 
 Advantages of Data Abstraction:
•	Helps the user to avoid writing the low level code
•	Avoids code duplication and increases reusability.
•	Can change internal implementation of class independently without affecting the user.
•	Helps to increase security of an application or program as only important details are provided to the user.

Encapsulation:- 
•	 Encapsulation is defined as wrapping up of data and information under a single unit. 
•	In Object-Oriented Programming, Encapsulation is defined as binding together the data and the functions that manipulate them.
•	Encapsulation also leads to data abstraction or hiding. As using encapsulation also hides the data.

Inheritance :- The capability of a class to derive properties and characteristics from another class is called Inheritance.
•	Sub Class: The class that inherits properties from another class is called Sub class or Derived Class.
•	Super Class:The class whose properties are inherited by sub class is called Base Class or Super class.
•	Reusability: Inheritance supports the concept of “reusability”, i.e. when we want to create a new class and there is already a class that includes some of the code that we want, we can derive our new class from the existing class. By doing this, we are reusing the fields and methods of the existing class.
•	we can simply avoid the duplication of data and increase re-usability using  inheritance.

Modes of inheritance.:
 
1.	Single Inheritance: one sub class is allowed to inherit from only one base class.
2.	Multiple Inheritance:  one sub class is inherited from more than one base classes.
3.	Multilevel Inheritance: a derived class is created from another derived class.
4.	Hierarchical Inheritance :more than one derived class is created from a single base class.
5.	Hybrid (Virtual) Inheritance: Hybrid Inheritance is implemented by combining more than one type of inheritance.
6.	A special case of hybrid inheritance : Multipath inheritance: 
   A derived class with two base classes and these two base classes have one common base class is called multipath inheritance. 
              •	An ambiguity can arrise in this type of inheritance. 
                  Avoiding ambiguity using scope resolution operator
                  Avoiding ambiguity using virtual base class: 

