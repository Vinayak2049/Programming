# Cat and Hat

## You are given a string str, you need to return True if  the words "cat" and "hat" appear same number of times in str, otherwise return False.

### Code (with using find())
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

### Code (without using find())
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
