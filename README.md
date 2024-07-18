# prime-number-between-given-number
#include<iostream>
using namespace std;
int main()
{
    int a ,b;
    cout<<"enter the value of a";
    cin>>a;
    cout<<"enter the value b";
    cin>>b;
    if(a>b)
    {
        cout<<"note a should be greater then b";
        return 1;
        
    }
    for(int num=a;num<=b;num++)
    {
        if(num<2)
        {
            continue;
        }
        bool isprime=true;
        for(int i=2;i<num/2;i++)
        {
            if(num%2==0)
            {
                isprime=false;
                break;
            }
        }
    
    if(isprime)
    {
        cout<<num<<endl;
    }
    }
    return 0;
}
