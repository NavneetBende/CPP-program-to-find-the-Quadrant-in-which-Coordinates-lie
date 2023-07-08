# CPP-program-to-find-the-Quadrant-in-which-Coordinates-lie

Quadrants in which coordinate lies in C
Here, we will discuss the program for Quadrants In Which Coordinates Lie in C. The C program reads the coordinate point in a x-y coordinate system and identify the quadrant. The program takes X and Y. On the basis of x and y value, the program will identify on which quadrant the point lies.

Shortest Job First Scheduling Non Preemptive
While loop in C
Working :
According mathematics quadrants rules:

X  is positive integer as well as Y is also positive a integer it signifies first quadrant.
X  is negative integer but Y is positive integer it signifies second quadrant.
X  is negative integer as well as Y is also negative integer it signifies third quadrant.
X  is positive integer but Y is negative integer it signifies fourth quadrant.
Algorithm :
Get value of x & y
If ( x>0 and y>0 ) First Quadrant
If ( x<0 and y>0 ) Second Quadrant
If ( x<0 and y<0 ) Third Quadrant
If ( x>0 and y>0 ) Fourth Quadrant
If ( x=0 and y=0 ) Origin
If ( x!=0 and y=0 ) x-axis
If ( x>0 and y>0 ) y-axis
Quadrant in which coordinate lie in C++
C++ code
Run
#include<bits/stdc++.h>
using namespace std;

int 
main () 
{

    //for initialization of coordinates
  int x, y;			//user input
  cout << "Insert the value for variable X and Y : "; cin >> x >> y;
  
 
 
    //find true condition of first quadrant 
    if (x > 0 && y > 0)
    
 
cout << "point " << x << ", " << y << " lies in the First quadrant\n";
  
 
 
    //find second quadrant
    else if (x < 0 && y > 0)
    
 
cout << "point " << x << ", " << y << " lies in the Second quadrant\n";
  
 
 
    //To find third quadrant
    else if (x < 0 && y < 0)
    
 
cout << "point " << x << ", " << y << " lies in the Third quadrant\n"; //To find Fourth quadrant else if (x > 0 && y < 0)
    
cout << "point " << x << "," << y << "lies in the Fourth quandrant\n";
  
    //To find dose not lie on origin 
    else if (x == 0 && y == 0)
    
cout << "point " << x << ", " << y << " on x-axix\n";
  
//On x-axis 
    else if (y == 0 && x != 0)
    
cout << "point " << x << ", " << y << " on x-axix\n";
  
    //On y-axis
    else if (x == 0 && y != 0)
    
cout << "point " << x << ", " << y << "on at y-axix\n";
  
return 0;
}
Output
Insert the value for variable X and Y : -3 -33
point (-3, -33) lies in the Third quadrant
