// reverse-a-number
#include <iostream>
#include <math.h>

using namespace std;
int reverse(int n){
    int rev,temp;
    while(n!=0){
        temp=n%10;
        rev= temp + 10*rev;
        n=n/10;
    }
    return rev;
}

int main()
{   
    int n, val=0;
   cout<<"enter the number: ";
   cin>>n;
   cout<<"reverse = "<<reverse(n);
  
    return 0;
}
