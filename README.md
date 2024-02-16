# OOPS-Notes

## Overview

### 1. C++ What is OOP?

OOP stands for Object-Oriented Programming.

Procedural programming is about writing procedures or functions that perform operations on the data, while object-oriented programming is about creating objects that contain both data and functions.

Object-oriented programming has several advantages over procedural programming:

OOP is faster and easier to execute
OOP provides a clear structure for the programs
OOP helps to keep the C++ code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug
OOP makes it possible to create full reusable applications with less code and shorter development time
Tip: The "Don't Repeat Yourself" (DRY) principle is about reducing the repetition of code. You should extract out the codes that are common for the application, and place them at a single place and reuse them instead of repeating it.

### 2. C++ What are Classes and Objects?

Classes and objects are the two main aspects of object-oriented programming.
A class is a template for objects, and an object is an instance of a class.

When the individual objects are created, they inherit all the variables and functions from the class.

### 3. How OOP is related to real world ?

You are familiar with OOP concept theoretically but if interviewer ask to tell the concept with OOP concept then a lot of us are fail to answer.

Basically why we are write coding ,to solve our real world problem right.
In OOP a logic is right base on the object with this features

*  abstraction
*  encapsulation
*  inheritance
*  polymorphism

There are a lot of Car,bike,ATM and coffee machine.and there brands and name also different.
In OOP those are called object.

Objects logic are done by classes for example ,by phone we can call,Bluetooth ,take photo etc. those every logic
will be divide as classes. When we are creating class we need consider about SOLID principle.

4 Major Pillars Of OOPs Concepts With Real Time Examples:-


**Encapsulation**, **abstraction**, **inheritance**, and **polymorphism** are the four essential concepts of object-oriented programming. Even if these notions appear to be quite complicated, understanding the broad structure in which they operate can aid you in comprehending the fundamentals of an OOP computer programme. We’ll go through these four fundamental principles of OOPs concepts with real time examples and what they encompass in more detail below:

**Encapsulation**

The word “encapsulate” refers to the act of enclosing something. Encapsulation works in OOP in a similar fashion to how a pill “encapsulates” or contains the medication under its coating: by building a protective barrier around the information contained within a class from the rest of the cod

In our topic of OOPs concepts with real time examples, we encapsulate data and methods that operate on it by combining them into a single unit, the class. We can hide private information of a class from the outside world and only disclose functionality that is needed to interact with it this way. We say a class is properly enclosed when it prevents calling code from accessing its private data directly.

> OOPs Concepts with Real Time Examples: Extending the person class example from before, the class may contain private data, such as “socialSecurityNumber,” that should not be disclosed to other program objects. Outside programmes would not have direct access to this data member because it was encapsulated as a private variable in the class, and it would remain safe within that person’s object. If a method called “bankTransaction()” is implemented in the person class to make, say, a bank transaction, that function might then access the “socialSecurityNumber” variable as needed. Such a class would effectively encapsulate a person’s personal information.

**Abstraction**

When you can isolate the interface of a class from its implementation and focus on the interface, it’s often easier to reason and create a program. This is similar to seeing a system as a “black box,” where understanding the nitty-gritty inner workings isn’t required to reap the benefits of using it.

Because we are abstracting away the gory implementation details of a class and just exposing a clean and easy-to-use interface via the class’ member methods, this process is called “abstraction” in OOPs concepts with real time examples. When utilized correctly, abstraction isolates the impact of code changes, ensuring that if something goes wrong, the change only affects the implementation details of a class and not the outside code.

* Abstraction using Classes: We may use classes to implement Abstraction in C++. Using the available access specifiers, the class assists us in grouping data members and member functions. A Class has the ability to control which data members are visible to the outside world and which are not.

* Abstraction in Header files: Investment banking and financial modeling Header files are another sort of abstraction that can be used in C++. Consider the pow() method in the math.h header file, for example. We just call the function pow() in the math.h header file whenever we need to calculate the power of a number and supply the numbers as arguments, without knowing the underlying algorithm through which the function calculates the power of numbers.

> Example: Consider a stereo system as an object with a sophisticated logic board on the inside. It features buttons on the outside that allow it to be interacted with. Because you can’t see what occurs on the inside when you press any of the buttons, you don’t think about it. Even if you can’t see the logic board conducting these activities as a result of hitting a button, it is doing so behind your back. In our blog of OOPs concepts with real time examples, this concept of abstraction, which is extremely valuable in all fields of engineering and can also be seen in action in object-oriented programming.


> OOPs Concepts With Real Time Examples:
For instance, in OOP, we might design a class to represent the human body. Some functions, such as “walk()” or “eatFood(),” could be defined as part of the public-facing interface. Calling programmes might call these functions while remaining fully naive to the human body’s intricate inner workings and the processes required to walk or eat. These specifics are totally concealed in the implementation of the walk() and eatFood() body methods, and so are abstracted from the end user. It isn’t necessary for calling code to understand how the brain coordinates walking or how the stomach regulates food digestion in these circumstances; rather, it is sufficient to know that a human moved or ate.

> OOPs concepts with Real Time Examples:
The man only knows that pressing the accelerators will increase the car’s speed and that applying the brakes will stop it, but he has no idea how the speed is increased by pressing the accelerators, nor does he understand the car’s inner mechanism or how the accelerator, brakes, and other controls are implemented in the car. This is the definition of abstraction.

**Inheritance**


The OOPs concepts with real time examples of “inheritance” are almost always supported by object-oriented languages that offer classes. Classes can be grouped into hierarchies, with each parent or child class having one or more children. If a class has a parent class, it is said to be derived or inherited from it, and it represents an “IS-A” relationship. That is, the parent class’s child class has the “IS-A” type.

As a result, if a class inherits from another class, it inherits a lot of the same functionality and properties, and it can be modified to contain different code and data. Because the functionalities of a parent class do not need to be re-defined in any of its child classes, inheritance generally leads to good code reuse.

Consider two classes, one of which is the superclass (or parent), and the other is the subclass (or child). The parent class’s properties will be passed down to the child class, which may be modified or extended. Programmers that use the inheritance approach group these classes into what is known as a “IS-A” connection.

> Real Time Example: An insect could be represented by an Insect superclass in the animal world. Insects all have the same characteristics, such as six legs and an exoskeleton. For grasshoppers and ants, subclasses could be created. They inherently share all bug features because they inherit or are derived from the Insect class.

**Polymorphism**


In our topic of OOPs concepts with real time examples, Polymorphism is an OOP feature that allows classes in a hierarchy to be treated the same way. As a result, calling code only needs to handle objects from the hierarchy’s root, and each object instantiated by any child class is treated the same way.

Because derived objects and their parents have the same interface, the caller code can utilize any function in that class’ interface. Depending on the type of object supplied, the appropriate function will be invoked at run-time, resulting in potentially various behavior.

> OOPs, Concepts With Real Time Examples: Assume we have an “Animal” class with two child classes named “Cat” and “Dog.” We can override the “makeNoise” function that is inherited by the subclasses “Cat” and “Dog” to be “meow” and “bark,” respectively if the Animal class contains a way to create a noise named “makeNoise.” Then, another function may be built that takes any Animal object as a parameter and calls the “makeNoise” member function on it. Depending on the type of animal object that was supplied to the function, the noise will be either a “meow” or a “bark.”


### 4. Why to study OOPs ?

1. Duplicate code is a Bad.

2. Code will always be changed.

So, above statement proves, OOPs is provides code reusability which reduce the duplication of code because once you have duplicate code, you have make changes everywhere which leads to performance. Code can be changed anytime or requirement of application changed anytime so when you want to make changes in your application, OOPs makes it easier.

### 5. Advantages of OOPS

1. Improved software-development productivity: Object-oriented programming is
modular, as it provides separation of duties in object-based program development. It
is also extensible, as objects can be extended to include new attributes and
behaviors. Objects can also be reused within an across applications. Because of
these three factors – modularity, extensibility, and reusability – object-oriented
programming provides improved software-development productivity over traditional
procedure-based programming techniques.


2. Improved software maintainability: For the reasons mentioned above, objectoriented software is also easier to maintain. Since the design is modular, part of the
system can be updated in case of issues without a need to make large-scale
changes.

3. Faster development: Reuse enables faster development. Object-oriented
programming languages come with rich libraries of objects, and code developed
during projects is also reusable in future projects.

4. Lower cost of development: The reuse of software also lowers the cost of
development. Typically, more effort is put into the object-oriented analysis and
design, which lowers the overall cost of development.


5. Higher-quality software: Faster development of software and lower cost of
development allows more time and resources to be used in the verification of the
software. Although quality is dependent upon the experience of the teams, objectoriented programming tends to result in higher-quality software.

### 6. Limitations of OOPS

1. Steep learning curve: The thought process involved in object-oriented programming
may not be natural for some people, and it can take time to get used to it. It is
complex to create programs based on interaction of objects. Some of the key
programming techniques, such as inheritance and polymorphism, can be
challenging to comprehend initially.

2. Larger program size: Object-oriented programs typically involve more lines of code
than procedural programs.

3. Slower programs: Object-oriented programs are typically slower than procedurebased programs, as they typically require more instructions to be executed.

4. Not suitable for all types of problems: There are problems that lend themselves well
to functional-programming style, logic-programming style, or procedure-based
programming style, and applying object-oriented programming in those situations will
not result in efficient programs. 


### 7. When we say that "X" language is object oriented programming language, then what does we mean by that ?
If it is written in terms of objects and classes. And it follows all the OOPS concepts 


## Classes

###  1. Difference between Structure and Class

| Structure   |      Class      |  
|----------|:-------------:|
| 1. Members of a class are private by default.|	1. Members of a structure are public by default. |
|2. An instance of a class is called an ‘object’.|	2. An instance of structure is called the ‘structure variable’.|
|3. Member classes/structures of a class are private by default but not all programming languages have this default behavior eg Java etc.|	3. Member classes/structures of a structure are public by default.|
|4. It is declared using the class keyword.|	4. It is declared using the struct keyword.|
|5. It is normally used for data abstraction and further inheritance.|	5. It is normally used for the grouping of data|
|6. NULL values are possible in Class.|	6. NULL values are not possible.|
 
|7. Structure Syntax:  class class_name{
                           data_member;
                           member_function;
                  };|
|7. Class Syntax: struct structure_name{
                  type structure_member1;
                  type structure_member2;
                  }; |   


