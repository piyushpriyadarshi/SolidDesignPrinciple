# Solid Design Principle

| Principle                       | Description                                                                                                 |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| Single Responsibility Principle | Each class should be responsible for a single part or functionality of the system . That is so funny! :joy: |
| Open Closed Principle           | Software components should be open for extension, but not for modification.                                 |
| Liskov Substitution Principle   | Objects of a superclass should be replaceable with objects of its subclasses without breaking the system.   |
| Interface Segregation Principle | No client should be forced to depend on methods that it does not use.                                       |
| Dependency Inversion Principle  | High-level modules should not depend on low-level modules, both should depend on abstractions.              |

## Single Responsibility

```java
public class ParkingLot {
    public String park(Vehicle vehicle){

    }
    public String unPark(Vehicle vehicle){

    }
}


```

## Open Closed

```java

public interface ParkingPrice{
    public int calculatePrice();
}

public abstract class Vehicle {
    private Engine engine;

    private Engine getEngine(){
        return this.engine;
    }
    public abstract getNumberOfWheels();
}


public class Car extends Vehicle implements ParkingPrice{
    public int calculatePrice(){
        return this.getNumberOfWheels()*10;
    }
    public int getNumberOfWheels(){
        return 4;
    }
}

public class Bike extends Vehicle implements ParkingPrice{
    public int calculatePrice(){
        return this.getNumberOfWheels()*10;
    }
    public int getNumberOfWheels(){
        return 2;
    }
}
```

## Interface Segregation Principle

```java




```
