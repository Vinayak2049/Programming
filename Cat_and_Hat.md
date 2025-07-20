# You are given a string str, you need to return True if  the words "cat" and "hat" appear same number of times in str, otherwise return False.

## Python Code (with using find()):
  def cat_hat(str):
    cat_count=str.count("cat")
    hat_count=str.count("hat")
    if cat_count == hat_count:
      return True
    else:
      return False

  str = input("Enter a string: ")
  cathat = cat_hat(str)
  print(cathat)

## Python Code (without using find()):
  def cat_hat(str):
    cat = 0
    hat = 0
    for i in range(len(str)-2):
      string = str[i:i+3]
      if string == "cat":
          cat = cat + 1
      elif string == "hat":
          hat = hat +1
    return cat == hat

  str = input("Enter a string: ")
  cathat = cat_hat(str)
  print(cathat)


## C Code:

#include<stdio.h>
#include<string.h>
int main(){
    char str[100];
    int cat = 0;
    int hat = 0;
    printf("Enter a string: ");
    scanf("%s",str);
    char *ptr = str;
    while((ptr=strstr(ptr,"cat"))!= NULL){
        cat++;
        ptr=ptr+1
    }
    ptr = str;
    while((ptr=strstr(ptr,"hat"))!= NULL){
        hat++;
        ptr=ptr+1
    }
    if(cat==hat)
    printf("True");
    else
    printf("False");
    return 0;
}
