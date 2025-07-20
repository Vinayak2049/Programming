# Given two integer variables a and b, and a boolean variable flag. The task is to check the status and return accordingly.

   Return True for the following cases:

   Either a or b (not both) is non-negative and the flag is false.
   Both a and b are negative and the flag is true.
   Otherwise, return False.

## Python Code:
def checkStatus(a, b, flag):
        if a>=0 and b<=0 and flag == False:
            return True
        elif a<=0 and b>=0 and flag == False:
            return True
        elif a<=0 and b<=0 and flag == True:
            return True
        else:
            return False
            
a = int(input("Enter a number: "))
b = int(input("Enter a number: "))
flag = int(input("Enter 0 or 1: "))
status=checkStatus(a,b,flag)
print(status)


## C Code:

#include <stdio.h>

int Status(int a, int b, int flag) {
    if ((a < 0 || b < 0) && flag == 0) {
        return 1;
    }
    else if (a < 0 && b < 0 && flag == 1) {
        return 1;
    }
    else {
        return 0;
    }
}

int main() {
    int a, b;
    int flag;
    printf("Enter a number: ");
    scanf("%d", &a);
    printf("Enter a number: ");
    scanf("%d", &b);
    printf("Enter 0 or 1: ");
    scanf("%d", &flag);
    if (Status(a, b, flag)) {
        printf("True\n");
    } else {
        printf("False\n");
    }
    return 0;
}

