# Given a positive integer x. Your task is to check, if it is even or odd

## Python Code:

def checkOddEven(x):
    if (x % 2 == 0):
        print("Even")
    else:
        print("Odd")
        
x = int(input("Enter a Number: :))
checkOddEven(x)


## C Code:

#include<stdio.h>

int Even_Odd(int x){
    if (x%2==0){
        printf("Even");
    }
    else{
        printf("odd");
    }
}

int main(){
    int x;
    printf("Enter a number: ");
    scanf("%d",&x);
    Even_Odd(x);
}


## C++ Code:

#include <iostream>

int main()
{
    int num;
    std::cout<<"Enter a number: ";
    std::cin>>num;
    if(num%2==0){
        std::cout<<"Even";
    }
    else{
        std::cout<<"Odd";
    }
    return 0;
}
