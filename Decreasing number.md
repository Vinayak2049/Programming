# Given a number x, the task is to print the numbers from x to 0 in decreasing order in a single line.

## Python code:
x = int(input("Enter a number: "))
while(x>=0):
    print(x,end=' ')
    x=x-1


## C Code:
#include<stdio.h>

int main(){
    int x;
    printf("Enter a Number: ");
    scanf("%d",&x);
    while(x>=0){
        printf("%d ",x);
        x--;
    }
    return 0;
}


## C++ Code:
#include<iostream>

int main(){
    int x;
    std::cout<<"Enter a number: ";
    std::cin>>x;
    while(x>=0){
        std::cout<<x<<" ";
        x--;
    }
    return 0;
}
