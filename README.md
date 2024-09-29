# Experiment-11
## Aim:-
To study and implement Classes and Objects

## Apparatus:-
Vs Code

## Theory:-
#### Class: A blueprint for creating objects. It defines a data structure by combining data (attributes) and methods (functions) that operate on the data.Class Definition: A class is defined using the class keyword followed by the class name and a block of code that includes its attributes and methods.
#### Object: An instance of a class. It represents a specific realization of the class, holding actual values for the attributes defined by the class.An object is created by instantiating the class. This involves calling the class as if it were a function. Sure! Here's a detailed explanation of the concepts related to classes and objects, including definitions, syntax, access specifiers, and variable types.

#### Access Specifiers Comparison
Access specifiers determine the visibility and accessibility of class members (attributes and methods).
Access Specifier	Definition	Visibility	Example Usage
1. Public	Members are accessible from outside the class.	Unrestricted access.	self.attribute1
2. Private	Members are accessible only within the class.	Restricted access (prefix with __).	self.__attribute1
3. Protected	Members are accessible within the class and subclasses.	Limited access (prefix with _).	self._attribute1

#### Global and Local Variables
1. Global Variables:
Definition: Variables declared outside of any function or class. They are accessible from any part of the program.
Scope: Entire program.

2. Local Variables:
Definition: Variables declared within a function or block. They are only accessible within that function or block.
Scope: Limited to the function or block where they are declared.

## Codes:-
1.
```
//ashu
//Prn: 23070123154 
//experiment 11: 

#include <iostream>
using namespace std;

class cube
{
    public:
    int height = 2;
    int width = 3;
    int length = 5;
};

int main()
{
    cube c1;
    int vol = c1.height*c1.width*c1.length;
    cout<<"volume:"<<vol<<endl;
}
```
2.
```
   //Ashu yadav 
//Prn: 23070123154 
//experiment 11: 

#include <iostream>
using namespace std;

class cube
{
    public:
    int height = 2;
    int width = 2;
    int length = 2;
    int volume()
    {
        int v; 
        v = height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    cout<<"volume: "<<cube1.volume()<<endl;
}
```
3.
```
// Ashu yadav
// Prn: 23070123154 
// Experiment 11:

#include <iostream>
using namespace std;

class Cube {
    private:
        int height = 4;  
        int width = 2;   
        int length = 2; 

    public:
         
        double volume() {
            
            return static_cast<double>(height * width * length);
        }
};

int main() {
    Cube cube1;  
    cout << "Volume: " << cube1.volume() << endl;
    return 0;  
}
```
4. 
```
// Ashu yadav
// Prn: 23070123154
// Experiment 11:
#include<iostream>
using namespace std;
class cube{
    public:
    double height=1.2;
    double width=2.5;
    double length=3.8;
     double volume(){
     double v;
     v=height*width*length;
        return v;
}
void disp_vol(double vol){
    cout<<"Volume:"<<vol<<endl;

}
};
int main()
{
    cube cube1;
    double vol=cube1.volume();
    cube1.disp_vol(vol);
}
```
5. 
```
// Ashu yadav
// Prn: 23070123154
// Experiment 11:

#include <iostream>
using namespace std;

class Volume {
    public:
        float length;
        float breadth;
        float height;
        
       
        void input() {
            cout << "Enter the value of length: ";
            cin >> length;
            cout << "Enter the value of breadth: ";
            cin >> breadth;
            cout << "Enter the value of height: ";
            cin >> height;
        }

       
        float vol() {
            return length * breadth * height;
        }

      
        void display() {
            float volume = vol();
            cout << "The volume is " << volume << endl;
        }
};

int main() {
    Volume volume1; 
    volume1.input();  
    volume1.display(); 
    return 0;          
}
```
## Output:- 
1. ![image](https://github.com/user-attachments/assets/87910c25-d52e-4be0-94ea-4051d400f5cf)
2. ![image](https://github.com/user-attachments/assets/9744203c-eeda-4bdf-b79c-c87e0e149bc0)
3. ![image](https://github.com/user-attachments/assets/c2a2316a-5e04-44cc-8aa0-2f4c929f748b)
4. ![image](https://github.com/user-attachments/assets/46099362-589a-42fd-8711-b00bee95828e)
5. ![image](https://github.com/user-attachments/assets/98370d69-f26e-4eca-97d3-4247e1a627d9)


# Conclusion:-
1. Classes define the structure and behaviors of objects. They encapsulate data and methods into a single unit.
2. Objects are instances of classes and hold specific data values.
3. Access Specifiers (Public, Private, Protected) control how and where class members can be accessed and modified.
4. Global Variables are accessible throughout the entire program, while Local Variables are restricted to the function or block where they are defined.




