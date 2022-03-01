# shortest-path
/******************************************************************************

Welcome to GDB Online.
GDB online is an online compiler and debugger tool for C, C++, Python, PHP, Ruby, 
C#, VB, Perl, Swift, Prolog, Javascript, Pascal, HTML, CSS, JS
Code, Compile, Run and Debug online from anywhere in world.

*******************************************************************************/
#include<iostream>
#include<math.h>
using namespace std ;
int main()
{
    string s= "SWENNSEESS";
    int up = 0 , right = 0;
    for(int i = 0;i<s.length();i++)
    {
        if(s[i]=='E') right++;
       else  if(s[i]=='W') right--;
        else if(s[i]=='S') up--;
        else if(s[i]=='N') up++;
      
        
    }
    if(right<0) right+=right;
    if(up<0) up+=up;
        float a = float(right*right);
       float b = float(up*up);
        
        float c = sqrt(a+b);
cout<<c;
    return 0;
}
