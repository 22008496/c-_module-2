
# EX.NO : 2(A)  C++ DYNAMIC MEMORY ALLOCATION  

# PROGRAM STATEMENT :  
To write a CPP Program to allocate memory dynamically for a integer variable. (Note: p_var =  new typename;)  
# ALGORITHM :  
1. Start the program.  
2. Define a class var_space with a method allocateSpace that dynamically allocates memory for a  integer, reads a value from the user, and prints it.  
3. In the main function, create an object of var_space and call allocateSpace.  
4. End the program.

# PROGRAM :  
```
#include <iostream>

int main() {
    int* p_var = new int;
    std::cin >> *p_var;
    std::cout << "Integer Value is : " << *p_var << std::endl;
    delete p_var;
    return 0;
}
```
# output:

![Screenshot 2025-05-27 094746](https://github.com/user-attachments/assets/9a475cd7-e471-4ef9-ac59-a2884a463c26)

# Result:

Thus, the C++ program to allocate memory dynamically for a integer variable is created  successfully. 
