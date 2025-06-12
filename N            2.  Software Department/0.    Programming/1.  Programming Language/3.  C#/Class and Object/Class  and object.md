
### Class

- **Definition**: A class in C# is a blueprint or template for creating objects. It defines a datatype by bundling data and methods that work on the data into one single unit. A class can include fields, properties, methods, and events.
					`or`
  A **class** is a blueprint for creating objects.

- **Static Entity**: A class is a static entity, which means it exists in your source code and in the compiled code, but it does not occupy memory by itself until an object is created.
    
```

    
    public class Car
     {  
            `public string Make;` 
            `public string Model;`    
            `public int Year;`      // Constructor     
            public Car(string make, string model, int year) 
                {   
                      `this. Make = make;`     
                         `this.Model = model;`    
                              `this. Year = year;`  
               }      
                   
                public void DisplayInfo()   
                  {       
                    Console. WriteLine($"Car: {make} {model} ({year})");    
                  } 
    }`
```

### Object

- **Definition**: An object in C# is an instance of a class. When a class is instantiated, an object is created in memory.
- **Runtime Entity**: An object is a runtime entity, meaning it is created at runtime when the program is executed. It occupies memory and can be interacted with through its methods and properties.
- 
    
```
Car class Car myCar = new Car("Toyota", "Corolla", 2020); 
 myCar.DisplayInfo(); 
```
    

### Relationship Between Class and Object

- A **class** is a **definition** or a **template**, and it does **not** **consume** **memory** on its own.
- An **object** is an **instance** of a **class** and is created **in memory** when the **program** is **running**.
- The class defines what properties and methods its objects will have, but it is the creation of an object that brings those properties and methods to life, allowing them to be used in the program.

### Key Points

- **Classes** define the structure and behavior (data and methods) that the objects created from the class will have.
- **Objects** are concrete instances of classes that live in memory and can perform operations defined by their class.

