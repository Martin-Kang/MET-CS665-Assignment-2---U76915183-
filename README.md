# MET-CS665-Assignment 2-U76915183-Zeyu Kang

# GitHub Repo Link

https://github.com/Martin-Kang/MET-CS665-Assignment-2---U76915183-

# Design Pattern

The Design Pattern I used in my implementation is Observer Pattern -- When one delivery request(subject) is created, it will notify all the drivers(observers).


# How flexible is my implementation

It's easy to make some changes to my implementation. For example, it's easy to add another type of driver. Right now I have two types -- van driver and taxi driver, when we need to add another type, e.g. truck driver, we can 
just simplify inherit from the abstract class 'Driver' and materialize detailed functions in the new 'TruckDriver' class. 



# How is the simplicity and understandability of my implementation?

For my design, I mainly used five Classes -- Shop, DeliveryRequest, abstract classes Driver, and its concrete class VanDriver and TaxiDriver. The logic between them is also easy to understand. 
When a store creates an order, a delivery request for that order will be created. And then the request will be sent to all drivers.



# How did I avoid duplicated code?

To avoid duplicated code, I used abstract classes to represent all types of drivers. And when it comes to concrete driver type, I just need to inherit that abstract class and then add some specific functions and in this case
of my assignment 2, I just overrode the function of the abstract class.



# How to compile and run my implementation?


One choice is using IDE, e.g. IntelliJ IDEA. Import my project and open the Main.java and choose your JDK to compile it and run the main() function.


Another choice is typing command lines:


# Compile: 

```bash
mvn clean compile
``` 

# Run:

```bash
mvn -q clean compile exec:java -Dexec.executable="edu.bu.met.cs665.Main" -Dlog4j.configuration="file:log4j.properties"
```


