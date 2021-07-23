

<h1 align="center">OBJECT ORIENTED PROGRAMMING</h1>
<ul>
<li>The main aim of OOP is to bind together the data and the functions that operate on them so that no other part of the code can access this data except that function.</li>
<li>Object-oriented programming aims to implement real-world entities like inheritance, hiding, polymorphism, etc in programming.</li>
 </ul>
<h3 >Characteristics of an Object Oriented Programming language:</h3>
<br>
<b><u>CLASS </u> </b> : Class in C++ is a blue-print representing a group of objects which shares some common properties and behaviours.
<ul>
<li>A Class is a user-defined data-type which has data members and member functions which can be accessed and used by creating an instance of that class. </li>
<li>Data members are the data variables and member functions are the functions used to manipulate these variables and together these data members and member functions define the properties and behaviour of the objects in a Class.</li>
 <li>Member functions are method to access data memebers</li>
</ul>
<br>
<b> <u>OBJECTS</u> </b>:- An Object is an identifiable entity with some characteristics and behaviour. An Object is an instance of a Class
 When a class is defined, no memory is allocated but when it is instantiated (i.e. an object is created) memory is allocated.
 
 <br>
<b> Access Modifier </b>: Access Modifiers or Access Specifiers in a class are used to assign the accessibility to the class members. That is, it sets some restrictions on the class  members not to get directly accessed by the outside functions.
   3 types of access modifier:
   <ul>
<li>	Public : The data members and member functions declared as public can be accessed by other classes and functions too </li>
<li>Private: They are not allowed to be accessed directly by any object or function outside the class.  can be accessed only by the member functions inside the class </li>
<li>Protected : similar to private access modifier the difference is that the class members declared as Protected can be accessed by any subclass(derived class) of that class as well. </li>
 <li>by default the access modifier for the members will be Private.</li>
 </ul>
Only the member functions or the friend functions are allowed to access the private data members of a class.
 <u>Friend Class</u>
     A friend class can access private and protected members of other class in which it is declared as friend.
<br>
<b>Friend function</b>:  
<ul>
<li>Friends should be used only for limited purpose. too many functions or external classes are declared as friends of a class with protected or private data</li>
 <li>it lessens the value of encapsulation of separate classes in object-oriented programming </li>
 <li> A friend function can be </li>
a) A member of another class 
b) A global function 

<li>Friendship is not mutual. If class A is a friend of B, then B doesn’t become a friend of A automatically</li>
 </ul>
<br>
<b>POLYMORPHISM</b>
<ul>
 <li>polymorphism as the ability of a message to be displayed in more than one form.</li>
 <li>Polymorphism is extensively used in implementing inheritance</li>

<li>An operation may exhibit different behaviours in different instances. The behaviour depends upon the types of data used in the operation.</li>
 <li>C++ supports operator overloading and function overloading.</li>
 <ul>
 <li>Operator Overloading: The process of making an operator to exhibit different behaviours in different instances is known as operator overloading.</li>
 <li>Function Overloading: Function overloading is using a single function name to perform different types of tasks.</li>
 </ul>

 <li> <b>Compile time polymorphism </b>: This type of polymorphism is achieved by function overloading or operator overloading.</li>

1.function overloading: When there are multiple functions with same name but different parameters then these functions are said to be overloaded

2.Operator overloading: C++ has the ability to provide the operators with a special meaning for a data type, this ability is known as operator overloading.
 <ul>
<li>Almost all operators can be overloaded except few. Following is the  list of operators that cannot be overloaded.</li>
  <li>	. (dot) </li>
  <li>:: </li>
  <li>	?: </li>
  <li>	sizeof </li>
 </ul>
 <li><b>Runtime polymorphism</b>: This type of polymorphism is achieved by Function Overriding.</li>
•	Function overriding :when a derived class has a definition for one of the member functions of the base class. That base function is said to be overridden.
 <li> Runtime Plolymorphism used  virtual functions </li>
 <li> Virtual functions are used with inheritance, they are called according to the type of object pointed or referred, not according to the type of pointer or reference.  Virtual keyword is used to make a function virtual.</li>

Following things are necessary to write a C++ program with runtime polymorphism (use of virtual functions)
1) A base class and a derived class.
2) A function with same name in base class and derived class.
3) A pointer or reference of base class type pointing or referring to an object of derived class.
</ul>
<br>

<b>ABSTRACTION</b>
<ul>
<li>Data abstraction refers to providing only essential information about the data to the outside world, hiding the background details or implementation.</li>
<li>Abstraction using Classes: The class helps us to group data members and member functions using available access specifiers. A Class can decide which data member will be visible to the outside world and which is not</li>
 <li>Abstraction in Header files</li>
 </ul>
<b> Advantages of Data Abstraction</b>
<ul>
 <li>Helps the user to avoid writing the low level code</li>
 <li>Avoids code duplication and increases reusability </li>
 <li>Can change internal implementation of class independently without affecting the user</li>
<li>Helps to increase security of an application or program as only important details are provided to the user</li>
</ul>
<br>
<b>ENCAPSULATION</b> 
<ul>
 <li>Encapsulation is defined as wrapping up of data and information under a single unit. </li>
<li>In Object-Oriented Programming, Encapsulation is defined as binding together the data and the functions that manipulate them.</li>
<li>Encapsulation also leads to data abstraction or hiding. As using encapsulation also hides the data.</li>
</ul>
<br>

<b>INHERITANCE</b>
<ul>
 <li>The capability of a class to derive properties and characteristics from another class is called Inheritance.</li>
<li>Sub Class: The class that inherits properties from another class is called Sub class or Derived Class.</li>
<li>Super Class:The class whose properties are inherited by sub class is called Base Class or Super class.</li>
<li>Reusability: Inheritance supports the concept of “reusability”, i.e. when we want to create a new class and there is already a class that includes some of the code that we want, we can derive our new class from the existing class. By doing this, we are reusing the fields and methods of the existing class.</li>
 <li>we can simply avoid the duplication of data and increase re-usability using  inheritance.</li>
</ul>
<b>Modes of inheritance</b>
 ![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/table-class.png)
 
1.	Single Inheritance: one sub class is allowed to inherit from only one base class.
2.	Multiple Inheritance:  one sub class is inherited from more than one base classes.
3.	Multilevel Inheritance: a derived class is created from another derived class.
4.	Hierarchical Inheritance :more than one derived class is created from a single base class.
5.	Hybrid (Virtual) Inheritance: Hybrid Inheritance is implemented by combining more than one type of inheritance.
6.	A special case of hybrid inheritance : Multipath inheritance: A derived class with two base classes and these two base classes have one common base class is called multipath inheritance. 
   <ul>An ambiguity can arrise in this type of inheritance. 
 <li>Avoiding ambiguity using scope resolution operator</li>
 <li> Avoiding ambiguity using virtual base class</li> 
</ul>
