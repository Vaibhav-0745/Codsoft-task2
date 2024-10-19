# Codsoft-task2
#include<iostream>
#include<conio.h>
#include<stdlib.h>

using namespace std;

void add(int &x,int &y){
    cout<<"\nAddition is : "<<x+y;
}

void sub(int &x,int &y){
    cout<<"\nSubstraction is "<<x-y;
}

void mul(int &x,int &y){
    cout<<"\nMultiplication is : "<<x*y;
} 

void div(double &x,double &y){
    cout<<"\nDivision is : "<<x/y;
}
int main(){
    int x,y;
    cout<<"\nEnter two numbers : ";
    cin>>x>>y;
    double a=x;
    double b=y;
    int choice;
    while (choice<=6)
    {
        cout<<"\n\n\t*******Operation Choices*******";
        cout<<"\n1.Addition : ";
        cout<<"\n2.Substraction : ";
        cout<<"\n3.Multiplication : ";
        cout<<"\n4.Division : ";
        cout<<"\n5.Re-enter choice : ";
        cout<<"\n6.Exit : ";

        cout<<"\n\nEnter your choice : ";
        cin>>choice;

        switch (choice)
        {
        case 1:add(x,y);
            break;
        case 2:sub(x,y);
            break;
        case 3:mul(x,y);
            break;
        case 4:div(a,b);
            break;
        case 5: cout<<"\nEnter two numbers : ";
                cin>>x>>y;
                a=x;
                b=y;
                break;
        case 6:exit(0);
            break;
        default:cout<<"\nInvalid Choice : ";
            break;
        }


    }    
    return 0;
    
}
