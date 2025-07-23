# Given a positive integer x, the task is to print the numbers from 1 to x in the order as 12, 22, 32, 42, 52, ... (in increasing order).

## Python Code:

x = int(input("Enter a number: "))
y=1
while(y<x):    
    num=y*y   
    if(num<=x):
        print(num,end=' ')
    y=y+1


## C Code:

#include<stdio.h>

int main(){
    int x;
    printf("Enter a number: ");
    scanf("%d",&x);
    int y=1;
    while(y<x){
        int num = y*y;
        if(num<=x){
            printf("%d ",num);
        }
        y=y+1;
    }
    return 0;
}



## C++ Code:
#include<iostream>

int main(){
    int x;
    std::cout<<"Enter a number: ";
    std::cin>>x;
    int y=1;
    while(y<x){
        int num = y*y;
        if(num<=x){
            std::cout<<num<<" ";
        }
        y=y+1;
    }
    return 0;
}



## Java Code:

import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int x = scanner.nextInt();
        int y=1;
        while(y<x){
            int num = y*y;
            if(num<=x){
                System.out.printf("%d ",num);
            }
            y=y+1;
        }    
    }
}
