# You are given a string s, you need to print its characters at even indices(index starts at 0).

## Python Code:

s = input("Enter a string: ")
print("The characters at even indices are: ",end='')
for i in range(0,len(s),2):
    print(s[i],end='')



## C Code:

#include <stdio.h>

int main() {
    char s[100];
    printf("Enter a string: ");
    scanf("%s", s);
    printf("The characters at even indices are: ");
    for (int i = 0; s[i] != '\0'; i++) {
        if (i % 2 == 0) {
            printf("%c", s[i]);
        }
    }
    return 0;
}



## C++ Code:

#include <iostream>

int main()
{
    std::string name;
    std::cout<<"Whats your name: ";
    std::cin>>name;
    std::cout<<"The characters at even indices are: ";
    for(int i=0;name[i]!='\0';i++){
        if(i%2==0){
            std::cout<<name[i];
        }
    }
    return 0;
}
