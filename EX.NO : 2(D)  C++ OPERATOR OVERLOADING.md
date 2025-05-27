
# EX.NO : 2(D)  C++ OPERATOR OVERLOADING

# PROGRAM STATEMENT :  
To write a CPP Program to overload the '-' operator i.e. a positive value should be turned into a negative value.

# ALGORITHM:    
1. Start the program.  
2. Define a class rep with integer variables v and v1, and overload the decrement operator (--) to perform custom operations.  
3. In the overloaded -- operator, double the value of v, assign it to v1, then subtract v1 from v and print the result.  
4. In the main function, create an object c1 of class rep, read an integer value into c1.v, and use the overloaded decrement operator on c1.  
5. End the program.  
  
PROGRAM: 
```
#include <iostream>
using namespace std;
class Number {
    private:
        int value;
    public:
        Number(int v = 0) : value(v) {}
        Number operator-() {
            value = -value;  
            return *this;
        }
        int getValue() const {
            return value;
        }
};

int main() {
    int num;
    cin >> num;
    Number obj(num);
    obj = -obj;  
    cout << obj.getValue() << endl;
    return 0;
}
```


# output:
![Screenshot 2025-05-27 102326](https://github.com/user-attachments/assets/14626a98-c6d5-47a4-bf43-13293a35bc3b)

# Result:

Thus, the C++ program to overload the '-' operator i.e. a positive value should be turned into a negative value is created successfully. 
