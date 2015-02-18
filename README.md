# Quadratic-formula-and-circle-collision
c++ code that solves quadratic equations and determines if two circles collide 
//CGalicia 02-12-2015 Quadratic 

#include <iostream> 
#include <math.h> 
using namespace std;
int main() 

{ 
	//variables are declared with the double 
	double A, B ,C ,x1, x2;
	// Ax^2 + Bx +C = 0
	cout<<"Enter value for A=";
	cin>>A; 
	cout<<"Enter value for B=";
	cin>>B;
	cout<<"Enter value for C=";
	cin>>C;

    if ((B*B-4*A*C)>0)
    { x1 = (-B + sqrt(B*B-4*A*C)) / (2*A); //one asnwer 
	  x2 = (-B- sqrt(B*B-4*A*C)) / (2*A); // other asnwer 
      cout<<"The solutions are "<<x1<<" and " <<x2<<endl; //solution
	}
	
	else if ((B*B -4*A*C) == 0)
	{ x1 = (-B + sqrt(B*B-4*A*C)) / (2*A); // one asnwer 

	cout<<"The solution is"<<x1<<endl; // solution for problem
	}
	else 
	cout<<"There are no real solutions!"<<endl; // final statement 
	
    system ("pause"); //program is paused 
	return 0;
}
	
