
# EX.NO : 2(C)  C++ FUNCTION OVERLOADING 
# PROGRAM STATEMENT :  
To write a CPP program to overload a function to print Integer data in one and Floating-Point data in another.

# ALGORITHM :  
1. Start the program.  
2. Define a class print with a method dat overloaded to accept either an integer or a float, printing  each with a respective label.  
3. In the main function, declare an integer a and a float b, and read their values from the user.  
4. Create an object p of the print class, and call the overloaded dat method to print the integer and float values.  
5. End the program.

# Program:
```
#include <iostream> 
using namespace std; 
void printData(int x) { 
  cout << "Integer=" << x << endl; 
} 
void printData(float x) { 
   cout << "Floating Point=" << x << endl; 
} 
int main() { 
  int integerVal; 
  float floatVal; 
  cin >> integerVal >> floatVal; 
  printData(integerVal);     
  printData(floatVal);       
  return 0; 
}
```

# output:

![Screenshot 2025-05-27 101836](https://github.com/user-attachments/assets/092a13cd-8711-41c2-b3e4-90ac9f3c4ac9)

# Result:

Thus, the C++ program to overload a function to print Integer data in one and Floating- Point data in another is created successfully. 
