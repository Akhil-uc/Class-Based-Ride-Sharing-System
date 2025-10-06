# Class-Based-Ride-Sharing-System
Class-Based Ride Sharing System
This project demonstrates a class-based ride-sharing system implemented in Smalltalk and C++. It highlights Object-Oriented Programming (OOP) concepts such as Encapsulation, Inheritance, and Polymorphism. The system features three main classes: Ride, Driver, and Rider, with subclasses StandardRide and PremiumRide. The implementation emphasizes modular design, secure data management, code reuse, and adaptability, supporting future system expansions.


# How the Program Works
The program simulates a basic ride-sharing platform:

### Creates two types of rides:

StandardRide: costs $1.50 per unit distance
PremiumRide: costs $2.00 per unit distance


Creates a driver who can be assigned multiple rides
Creates a rider who can request multiple rides
Displays all requested rides with their details

Example:

Ride 1 (Standard): 10 units × $1.50 = $15.00
Ride 2 (Premium): 15 units × $2.00 = $30.00


# How It Should Be Implemented
Class Structure:
Ride (Base Class)

Contains: ride ID, pickup location, dropoff location, distance, fare
Has a method to calculate fare (can be overridden by subclasses)
Has a method to display ride details

StandardRide (Subclass)

Inherits from Ride
Calculates fare at $1.50 per unit distance

PremiumRide (Subclass)

Inherits from Ride
Calculates fare at $2.00 per unit distance

Driver Class

Contains: driver ID, name, rating, list of assigned rides
Can add rides to their assignment list
Can display driver information

Rider Class

Contains: rider ID, name, list of requested rides
Can request rides
Can view all their requested rides

## Why This Design?
Encapsulation: All data is private/protected and accessed through public methods
Inheritance: StandardRide and PremiumRide inherit common features from Ride, avoiding code duplication
Polymorphism: The fare calculation method works differently for each ride type, making it easy to add new ride types in the future

# OOP Concepts Demonstrated
1. Encapsulation

Class attributes are private/protected
Data is accessed only through public methods
Internal details are hidden from outside access

2. Inheritance

StandardRide and PremiumRide inherit from Ride
Common code is written once in the parent class
Subclasses reuse and extend parent functionality

3. Polymorphism

fareCalculation() method behaves differently for each ride type
Same method name, different implementations
Makes the code flexible and easy to extend
