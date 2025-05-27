
# EX.NO : 2(B)  C++ STATIC CLASS MEMBERS  

# PROGRAM STATEMENT :  

To write a CPP Program to create class Rectangle and calculate the volume of the rectangle, make  
use of static member variable in the class Rectangle.  

# ALGORITHM :  
1. Start the program.  
2. Define a class Rectangle with a static variable var to count the number of objects created. The  class includes a constructor to initialize length, breadth, and height, and a method Volume to  calculate the volume.  
3. In the main function, read two sets of dimensions from the user, create two Rectangle objects  with these dimensions, and display their volumes.  
4. Print the total number of Rectangle objects created using the static variable var.  
5. End the program.

# Program: 

```
#include <iostream> 
class Cuboid { 
private: 
    int length, breadth, height; 
    static int objectCount;  
public: 
    Cuboid(int l, int b, int h) { 
        length = l; 
        breadth = b; 
        height = h; 
        objectCount++;   
        std::cout << "Constructor called." << std::endl; 
    } 
    int volume() { 
        return length * breadth * height; 
    } 
    static int getObjectCount() { 
        return objectCount; 
    } 
}; 
int Cuboid::objectCount = 0; 
int main() { 
    int l1, b1, h1, l2, b2, h2; 
    std::cin >> l1 >> b1 >> h1; 
    Cuboid cuboid1(l1, b1, h1); 
    std::cout << "Volume :" << cuboid1.volume() << std::endl; 
    std::cin >> l2 >> b2 >> h2; 
    Cuboid cuboid2(l2, b2, h2); 
    std::cout << "Volume :" << cuboid2.volume() << std::endl; 
    std::cout << "Total objects: " << Cuboid::getObjectCount() << std::endl; 
    return 0; 
}
```

# Output: 

![Screenshot 2025-05-27 095337](https://github.com/user-attachments/assets/91ab400e-984d-4e68-b01d-7e60042d5e93)

# Result:

Thus, the C++ program to create class Rectangle and calculate the volume of the rectangle, make use of static member variable in the class Rectangle is created successfully. 
