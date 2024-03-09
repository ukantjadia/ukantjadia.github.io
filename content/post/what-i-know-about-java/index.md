---
title: What I Know About Java
subtitle: Me learning Java

summary: Me learning Java

draft: false
date: 2023-12-30T14:23:50+05:30
lastmod: 

categories:
    - Java
tags:
    - Java
    - Basics
projects: []
featured: false
# authors:
#   - Ukant Jadia


image:
  caption: ''
  focal_point: ''
  placement: 2
  preview_only: false
---



## Explaining the

```java
pubic static void main(String[] args)
```

- the execution of our code starts form main.
- let in order to create the object of class x we should have the main method

- So main is a parameter and it takes parameter ie. `main ( )`
- And the type of the parameter can be anything so we take the `string` because `String` except values and we don't know how many values we are taking so we take array `main(String args[])`

- There is nothing to return in main so it is a `void` type
- In order to call the method we require the object and the execution of our code is start from the main so that's why it considered as `static void main(String args[])`
- and it made public so `public static void main(String args[])`

### creating a object inside the main

- we type the class name and obj name `Main obj`
- then we have a keyword `new` : it tell the jvm how memory it required for the given class, for that the size of class is define by the default constructor.

+ it is like a blowing the air inside the pillow (keyword new ), and capacity of that pillow is constructor.

# Java OOP

## Method Overloading

- Methods with same name but diff in (parameter or data type of the(both)).
- this kind of methods are known as overloaded method.
ex :

```java
void func(){..}
int func(){...}
float func(int x){...}
void func(int x, float k, long l){...}
```

- Method overloading should be consider by the type or count of the parameter that passed to a method not by the **return type of the method.**

## Constructor
>
> - It is member method.
> - Constructor have same name as class name.
> - Constructor will never return anything.
> - It used to allocate the memory.
>
***
>
> - Every time when we have to create a any object we have to use the constructor weather we define it or not.
> - If we don't create a constructor it will be there that's a default constructor.
> - What a Constructor do : it will define the size of class which help keyword new to create the memory accordingly .

- unlike methods, a constructor has the **same name as that of class** and does not have any return type.
- In java similar to method but only invoked when an object of the class is created.
ex:

```java
class Main{
  private short num;

  // constructor
  Main() {
    System.out.println("After the object is create. ");
    num = 27;
  }

  public static void main(String[] args){
  // object of class is created 
  Main obj = new Main();
  // calling the var
  System.out.println("the short number is "+ obj.num);
  }
}
```

- There are three type of Constructor
- **Private Constructor** : Private constructor can't be accessed from outside the class.
- **No-Arg Constructor** :  Constructor that does not accept any arguments.
- **Parameterized Constructor** :  Constructor that accepts arguments.
- **Default Constructor** : Constructor that is automatically created by the Java compiler if it is not defined.

___

- A constructor can not be `abstract`, `static` or `final`

## Access Modifier

- It is helpful in the Encapsulation ( preventing the data from misuse and alter.).
- And to Control what part of program can access the members of a class.
- **Default** : Declarations are visible only within the package(package private).
- **Public** : This can be access by other class.
- **Private** : This can not be accessed by other class.
- **Protected** : Declarations are visible within the package or all subclasses.

- refer to this image [this](https://cdn.programiz.com/sites/tutorial2program/files/java-access-modifiers-public-private-protected-default_0.jpg)

## this key word

- this : refer to the current object inside a method or constructor.
- in other words: this is treating the variable with same name, differently according to there position/place.
- using this with getters and setters : in getters/setters we are using the same var name as in the program
- using this in constructor overloading
ex:

```java
class Complex {

    private int a, b;

    // constructor with 2 parameters
    private Complex( int i, int j ){
        this.a = i;
        this.b = j;
    }

    // constructor with single parameter
    private Complex(int i){
        // invokes the constructor with 2 parameters
        this(i, i); 
    }

    // constructor with no parameter
    private Complex(){
        // invokes the constructor with single parameter
        this(0);
    }

    @Override
    public String toString(){
        return this.a + " + " + this.b + "i";
    }

    public static void main( String[] args ) {
  
        // creating object of Complex class
        // calls the constructor with 2 parameters
        Complex c1 = new Complex(2, 3); 
    
        // calls the constructor with a single parameter
        Complex c2 = new Complex(3);

        // calls the constructor with no parameters
        Complex c3 = new Complex();

        // print objects
        System.out.println(c1);
        System.out.println(c2);
        System.out.println(c3);
    }
}
```

- passing this as an argument : - i also didn't get it. ask to sir

## final keyword

- final keyword means used to denote the constants and it can be used with variables,method and classes.
- final variable cannot be reinitialized with another value.
- the final method cannot be overridden.
- the final class cannot be extended.

## `instanceOf` operator

- used to check whether an object is an instance of class or not
- syntax `objectName instanceOf className;`

## Inheritance

- It allows to create a new class from an existing class.
- just inherit it from it's father class.

```java
class Main
{ 
    public static void main(String args[])
    { 
        child boy = new child();        

        boy.display();
    }
}

class parent{
    String color = "White";
    System.out.println("It is same like we get the traits from our parents, JDK or JVM also doing the same thing.");
    // it is same like we get the traits from our parents, JDK/JVM/java is also doing the same thing. 
}


// inherit from parents
class child extends parent{
    public void display(){
        System.out.println("The value for variable \'color\' is comming from the parent class.");
        System.out.println("Color of child is "+color);
    }
}
```
