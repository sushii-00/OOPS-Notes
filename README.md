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

| Class   |      Structure      |  
|----------|:-------------:|
| 1. Members of a class are private by default.|	1. Members of a structure are public by default. |
|2. An instance of a class is called an ‘object’.|	2. An instance of structure is called the ‘structure variable’.|
|3. Member classes/structures of a class are private by default but not all programming languages have this default behavior eg Java etc.|	3. Member classes/structures of a structure are public by default.|
|4. It is declared using the class keyword.|	4. It is declared using the struct keyword.|
|5. It is normally used for data abstraction and further inheritance.|	5. It is normally used for the grouping of data|
|6. NULL values are possible in Class.|	6. NULL values are not possible.|
 
> 7. Structure Syntax:
```
class class_name{
                           data_member;
                           member_function;
                  };
```

> 7. Class Syntax:

```
struct structure_name{
                  type structure_member1;
                  type structure_member2;
                  }; 
```
### 2. Similarities of classes and structures:

* Hold data members

One of the most fundamental similarities between classes and structures is that both can hold data members. Data members are variables that hold data associated with an object. In a class, data members are usually defined as private or protected, while in a structure, they are usually defined as public. However, the basic concept is the same for both - they provide a way to store data associated with an object.

* Provide member functions

Member functions are functions that operate on the data members of an object. In a class, member functions can be defined as public or private, while in a structure, they are usually defined as public. Once again, the basic concept is the same for both - they provide a way to operate on the data associated with an object.

* Support constructors

Constructors are special member functions that are used to initialize the data members of an object. Both classes and structures can support constructors. In a class, constructors can be defined as public or private, while in a structure, they are usually defined as public. However, the basic concept is the same for both - they provide a way to initialize the data associated with an object.

* Both can be passed as function arguments

Both classes and structures can be passed as function arguments. When passed as arguments, they are typically passed by reference. However, in some cases, they can also be passed by value. This means that they can be used interchangeably in many contexts.


* Used as templates

Templates are a powerful feature in C++ that allows classes and functions to be defined in a generic way. Both classes and structures can be used as templates. This means that they can be used to define generic data types and algorithms that can operate on different types of objects.

### 3. When to use Structure over Class


Do not define a structure unless the type has all of the following characteristics:

It logically represents a single value, similar to primitive types (integer, double, and so on).
It has an instance size smaller than 16 bytes.
It is immutable.
It will not have to be boxed frequently.

### 4. Access Modifiers

There are two types of modifiers in Java: access modifiers and non-access modifiers.

The access modifiers in Java specifies the accessibility or scope of a field, method, constructor, or class. We can change the access level of fields, constructors, methods, and class by applying the access modifier on it.

There are four types of Java access modifiers:

* **Private**: The access level of a private modifier is only within the class. It cannot be accessed from outside the class.
  
* **Default**: The access level of a default modifier is only within the package. It cannot be accessed from outside the package. If you do not specify any access level, it will be the default.
  
* **Protected**: The access level of a protected modifier is within the package and outside the package through child class. If you do not make the child class, it cannot be accessed from outside the package.
  
* **Public**: The access level of a public modifier is everywhere. It can be accessed from within the class, outside the class, within the package and outside the package.

**There are many non-access modifiers, such as static, abstract, synchronized, native, volatile, transient, etc. Here, we are going to learn the access modifiers only.**


**1) Private**
The private access modifier is accessible only within the class.

**Simple example of private access modifier**

In this example, we have created two classes A and Simple. A class contains private data member and private method. We are accessing these private members from outside the class, so there is a compile-time error.
```
class A{  
private int data=40;  
private void msg(){System.out.println("Hello java");}  
}  
  
public class Simple{  
 public static void main(String args[]){  
   A obj=new A();  
   System.out.println(obj.data);//Compile Time Error  
   obj.msg();//Compile Time Error  
   }  
} 
```

**Role of Private Constructor**
If you make any class constructor private, you cannot create the instance of that class from outside the class. For example:
```
class A{  
private A(){}//private constructor  
void msg(){System.out.println("Hello java");}  
}  
public class Simple{  
 public static void main(String args[]){  
   A obj=new A();//Compile Time Error  
 }  
}
```
**2) Default**


If you don't use any modifier, it is treated as default by default. The default modifier is accessible only within package. It cannot be accessed from outside the package. It provides more accessibility than private. But, it is more restrictive than protected, and public.

Example of default access modifier

In this example, we have created two packages pack and mypack. We are accessing the A class from outside its package, since A class is not public, so it cannot be accessed from outside the package.
```
//save by A.java  
package pack;  
class A{  
  void msg(){System.out.println("Hello");}  
}  
//save by B.java  
package mypack;  
import pack.*;  
class B{  
  public static void main(String args[]){  
   A obj = new A();//Compile Time Error  
   obj.msg();//Compile Time Error  
  }  
}

```
In the above example, the scope of class A and its method msg() is default so it cannot be accessed from outside the package.

**3) Protected**
The protected access modifier is accessible within package and outside the package but through inheritance only.

The protected access modifier can be applied on the data member, method and constructor. It can't be applied on the class.

It provides more accessibility than the default modifer.

Example of protected access modifier

In this example, we have created the two packages pack and mypack. The A class of pack package is public, so can be accessed from outside the package. But msg method of this package is declared as protected, so it can be accessed from outside the class only through inheritance.
```
//save by A.java  
package pack;  
public class A{  
protected void msg(){System.out.println("Hello");}  
}  
//save by B.java  
package mypack;  
import pack.*;  
  
class B extends A{  
  public static void main(String args[]){  
   B obj = new B();  
   obj.msg();  
  }  
}
```
> Output:Hello

**4) Public**
The public access modifier is accessible everywhere. It has the widest scope among all other modifiers.

Example of public access modifier
```
//save by A.java  
  
package pack;  
public class A{  
public void msg(){System.out.println("Hello");}  
}  
//save by B.java  
  
package mypack;  
import pack.*;  
  
class B{  
  public static void main(String args[]){  
   A obj = new A();  
   obj.msg();  
  }  
}  
```
> Output:Hello


**Java Access Modifiers with Method Overriding**

If you are overriding any method, overridden method (i.e. declared in subclass) must not be more restrictive.
```
class A{  
protected void msg(){System.out.println("Hello java");}  
}  
  
public class Simple extends A{  
void msg(){System.out.println("Hello java");}//C.T.Error  
 public static void main(String args[]){  
   Simple obj=new Simple();  
   obj.msg();  
   }  
} 
```
The default modifier is more restrictive than protected. That is why, there is a compile-time error.




### 5. Types of Class Member Functions in C++

We already know what member functions are, what they do, how to define member functions and how to call them using class objects. Now lets learn about some special member functions which can be defined in C++ classes. Following are the different types of Member functions:

* Simple functions
* Static functions
* Const functions
* Inline functions
* Friend functions

**1.) Simple Member functions in C++**
These are the basic member function, which dont have any special keyword like static etc as prefix. All the general member functions, which are of below given form, are termed as simple and basic member functions.

```
return_type functionName(parameter_list)
{
    function body;
}

```

**2.) Static Member functions in C++**
Static is something that holds its position. Static is a keyword which can be used with data members as well as the member functions. We will discuss this in details later. As of now we will discuss its usage with member functions only.

A function is made static by using static keyword with function name. These functions work for the class as whole rather than for a particular object of a class.

It can be called using the object and the direct member access . operator. But, its more typical to call a static member function by itself, using class name and scope resolution :: operator.

```
class X
{
    public:
    static void f()
    {
        // statement
    }
};

int main()
{
    X::f();   // calling member function directly with class name
}

```

These functions cannot access ordinary data members and member functions, but only static data members and static member functions can be called inside them.

It doesn't have any "this" keyword which is the reason it cannot access ordinary members. We will study about "this" keyword later.

**3.) Const Member functions in C++**
We will study Const keyword in detail later(Const Keyword), but as an introduction, Const keyword makes variables constant, that means once defined, there values can't be changed.

When used with member function, such member functions can never modify the object or its related data members.

```
// basic syntax of const Member Function

void fun() const 
{
    // statement
}

```


**4.) Inline functions in C++**
All the member functions defined inside the class definition are by default declared as Inline. We will study Inline Functions in details in the next topic.

**5.) Friend functions in C++**
Friend functions are actually not class member function. Friend functions are made to give private access to non-class functions. You can declare a global function as friend, or a member function of other class as friend.

```
class WithFriend
{
    int i;
    public:
    friend void fun(); // global function as friend
};

void fun()
{
    WithFriend wf;
    wf.i=10;  // access to private data member
    cout << wf.i;
}

int main()
{
    fun(); //Can be called directly
}

```

Hence, friend functions can access private data members by creating object of the class. Similarly we can also make function of some other class as friend, or we can also make an entire class as friend class.

```
class Other
{
    void fun();
};

class WithFriend
{
    private:
    int i;
    public:
    void getdata();  // Member function of class WithFriend
    
    // making function of class Other as friend here
    friend void Other::fun();   
    
    // making the complete class as friend
    friend class Other;  
};

```
When we make a class as friend, all its member functions automatically become friend functions.

**Friend Functions is a reason, why C++ is not called as a pure Object Oriented language. Because it violates the concept of Encapsulation.**


### 6. Constructors in C++
Constructor in C++ is a special method that is invoked automatically at the time of object creation. It is used to initialize the data members of new objects generally. The constructor in C++ has the same name as the class or structure. It constructs the values i.e. provides data for the object which is why it is known as constructor.

* Constructor is a member function of a class, whose name is same as the class name.

* Constructor is a special type of member function that is used to initialize the data members for an object of a class automatically, when an object of the same class is created.

* Constructor is invoked at the time of object creation. It constructs the values i.e. provides data for the object that is why it is known as constructor.
  
* Constructor do not return value, hence they do not have a return type.

```
The prototype of the constructor looks like 
    <class-name> (list-of-parameters);
 
```
**Constructor can be defined inside the class declaration or outside the class declaration**


**Example: defining the constructor within the class**
 ```
#include<iostream>
using namespace std;
class student
{
    int rno;
    char name[50];
    double fee;
    public:
    student()
    {
        cout<<"Enter the RollNo:";
        cin>>rno;
        cout<<"Enter the Name:";
        cin>>name;
        cout<<"Enter the Fee:";    
        cin>>fee;
    }    
     
 
 
    void display()
    {
        cout<<endl<<rno<<"\t"<<name<<"\t"<<fee;
    }
};
 
int main()
{
    student s;  //constructor gets called automatically when we create the object of the class
    s.display();
    return 0;
 
}

```


**Example: defining the constructor outside the class**
```
#include<iostream>
using namespace std;
class student
{
    int rno;
    char name[50];
    double fee;
    public:
    student();
    void display();
     
};
 
    student::student()
    {
        cout<<"Enter the RollNo:";
        cin>>rno;
        cout<<"Enter the Name:";
        cin>>name;
        cout<<"Enter the Fee:";    
        cin>>fee;
    }    
 
   void student::display()
    {
        cout<<endl<<rno<<"\t"<<name<<"\t"<<fee;
    }
     
int main()
{
    student s;
    s.display();
    return 0;
}

```

* **Characteristics of constructor**

    * The name of the constructor is same as its class name.
    * Constructors are mostly declared in the public section of the class though it can be declared in the private section of the class.
    * Constructors do not return values; hence they do not have a return type.
    * A constructor gets called automatically when we create the object of the class.
    * Constructors can be overloaded.
    * Constructor can not be declared virtual.
    * Constructor cannot be inherited.
    * Addresses of Constructor cannot be referred.
    * Constructor make implicit calls to new and delete operators during memory allocation.

* **Types of constructor**

    * Default constructor
    * Parameterized constructor
    * Overloaded constructor
    * Constructor with default value
    * Copy constructor
    * Inline constructor

* **A constructor is different from normal functions in following ways:** 

Constructor has same name as the class itself
Default Constructors don’t have input argument however, Copy and Parameterized Constructors have input arguments
Constructors don’t have return type
A constructor is automatically called when an object is created.
It must be placed in public section of class.
If we do not specify a constructor, C++ compiler generates a default constructor for object (expects no parameters and has an empty body).

**1. Default Constructors** : Default constructor is the constructor which doesn’t take any argument. It has no parameters. It is also called a zero-argument constructor.

```
  
// Cpp program to illustrate the
// concept of Constructors
#include <iostream>
using namespace std;
 
class construct {
public:
    int a, b;
 
    // Default Constructor
    construct()
    {
        a = 10;
        b = 20;
    }
};
 
int main()
{
    // Default constructor called automatically
    // when the object is created
    construct c;
    cout << "a: " << c.a << endl << "b: " << c.b;
    return 1;
}
```

> Output
a: 10
b: 20
> Note: Even if we do not define any constructor explicitly, the compiler will automatically provide a default constructor implicitly.


**2. Parameterized Constructors:** It is possible to pass arguments to constructors. Typically, these arguments help initialize an object when it is created. To create a parameterized constructor, simply add parameters to it the way you would to any other function. When you define the constructor’s body, use the parameters to initialize the object. 

> Note: when the parameterized constructor is defined and no default constructor is defined explicitly, the compiler will not implicitly call the default constructor and hence creating a simple object as

> Student s; //Will flash an error

```

// CPP program to illustrate
// parameterized constructors
#include <iostream>
using namespace std;
 
class Point {
private:
    int x, y;
 
public:
    // Parameterized Constructor
    Point(int x1, int y1)
    {
        x = x1;
        y = y1;
    }
 
    int getX() { return x; }
    int getY() { return y; }
};
 
int main()
{
    // Constructor called
    Point p1(10, 15);
 
    // Access values assigned by constructor
    cout << "p1.x = " << p1.getX()
         << ", p1.y = " << p1.getY();
 
    return 0;
}
```

> When an object is declared in a parameterized constructor, the initial values have to be passed as arguments to the constructor function. The normal way of object declaration may not work. The constructors can be called explicitly or implicitly.

> Example e = Example(0, 50); // Explicit call

> Example e(0, 50);           // Implicit call


**3. Copy Constructor: **
A copy constructor is a member function that initializes an object using another object of the same class. A detailed article on Copy Constructor.

Whenever we define one or more non-default constructors( with parameters ) for a class, a default constructor( without parameters ) should also be explicitly defined as the compiler will not provide a default constructor in this case. However, it is not necessary but it’s considered to be the best practice to always define a default constructor. 

Copy constructor takes a reference to an object of the same class as an argument.
