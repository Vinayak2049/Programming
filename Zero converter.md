# You are given a number n. The number n can be negative or positive. If n is negative, print numbers from n to 0 by adding 1 to n in the neg function. If positive, print numbers from n-1 to 0 by subtracting 1 from n in the pos function.

## Python Code:

def pos(n):
    for i in range(n-1,-1,-1):
            print(i,end=' ')
        
        
def neg(n):
    for i in range(n,1,+1):
            print(i,end=' ')
            

n = int(input("Enter a number: "))
if(n==0):
    print("Already zero")

elif(n>0):
    pos(n)

else:
    neg(n)


## C Code:

#include<stdio.h>

int pos(int n);
int neg(int n);

int pos(int n){
    for(int i=n-1;i>=0;i--){
        printf("%d ",i);
    }
}

int neg(int n){
    for(int i = n;i<=0;i++){
        printf("%d ",i);
    }
}


int main(){
    int n;
    printf("Enter a number: ");
    scanf("%d",&n);
    if(n==0){
        printf("Already zero");
    }
    else if(n>0){
        pos(n);
    }
    else{
        neg(n);
    }
    return 0;
}


## C++ Code:

#include<iostream>

int pos(int n);
int neg(int n);

int pos(int n){
    for(int i = n-1;i>=0;i--){
        std::cout<<i<<" ";
    }
    return 0;
}

int neg(int n){
    for(int i=n;i<=0;i++){
        std::cout<<i<<" ";
    }
    return 0;
}

int main(){
    int n;
    std::cout<<"Enter a number: ";
    std::cin>>n;
    if(n==0){
        std::cout<<"Already zero";
    }
    else if(n>0){
        pos(n);
    }
    else{
        neg(n);
    }
    return 0;
}



## Java Code:

import java.util.Scanner;


public class Main{
    public static void main(String[] args){
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = scanner.nextInt();
        if(n==0){
            System.out.println("Already zero");
        }
        else if(n>0){
            pos(n);
        }
        else{
            neg(n);
        }   
    }
    public static void pos(int n){
        for(int i=n-1;i>=0;i--){
            System.out.printf("%d ",i);
        }
    }
    public static void neg(int n){
        for(int i=n;i<=0;i++){
            System.out.printf("%d ",i);
        }
    } 
}
