# PTbac2
#include<iostream>
#include<stdio.h>
#include<cmath>
using namespace std;
int main(){
    int a,b,c;
    float D;
    cin>>a;
    cin>>b;
    cin>>c;
    D=b*b-4*a*c;
    if(a==0){
        if(b==0){
            if(c==0){cout<<"VSN";}
            else{cout<<"VN";}
        }
        else{printf("%.4f",(float)-c/b);}
    }
    if(a!=0){
        if(D<0){cout<<"VN";}
        else if(D==0){printf("%.4f",(float)-b/(2*a));}
        else{
            printf("%.4f",(float)(-b-sqrt(D))/(2*a));
            cout<<endl;
            printf("%.4f",(float)(-b+sqrt(D))/(2*a));
        }
    }
    return 0;
}
