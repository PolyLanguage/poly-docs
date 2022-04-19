# What is class? 
Class is basically structure that describes some object, it's describes its properties and functions. 

# Classes
To define a class in Poly language there's a keyword `class`, syntax of class definition:
```poly
class Car {} 
```

# Instances
As we know class is basically description of some object. Instance is that object, that was described by class. To create instance of class there's a `new` expression syntax:
```poly
class Car {} 

Car myCar = new Car();
```
Class is also a type of data, so we declare a variable with class type and create a instance of it with `new` expression. 

# Classes. Methods
You can define a methods of class inside class body, every instance of that class will hsve that method, so you can call it. Example:
```poly
class Car {
    method broom() {
        print('Broom broom!');
    }
}

Car myCar = new Car();
myCar.broom(); // Broom broom! 
```

Also you can define methods, that returns some stuff and accepts some arguments:
```poly
class Calculator {
    method int plus(int a, int b) {
        return a + b;
    } 
}

Calculator calc = new Calculator();
print(calc.plus(10, 10)); // 20
```

# Classes. Fields
Fields is basically variables of object. 
Theres a types of fields that limits its accessibility:
- `public` (get/set available for all scopes) 
- `visible` (get available for all scopes, set available only inside class methods) 
- `private` (get/set available only inside class methods)

Example:
```poly
class Car {
    field<public> int someField;
}

Car myCar = new Car();
myCar.someField = 123;
print(myCar.someField); // 123
```

# Classes. Constructor
Soon. 

# Classes. Context
Soon. 

# Classes. Inheritance
Soon. 
