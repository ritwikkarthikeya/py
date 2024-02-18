## Exercise: Python for loop
1. After flipping a coin 10 times you got this result,
```
result = ["heads","tails","tails","heads","tails","heads","heads","tails","tails","tails"]
```
Using for loop figure out how many times you got heads
ANSWER:
result = ["heads","tails","tails","heads","tails","heads","heads","tails","tails","tails"]
i="heads"
j=0
k=0
for j in range(len(result)):
     if (result[j]=="heads"):
      k=k+1
      j=j+1
     else:
      j=j+1   
print(k)

2. Print square of all numbers between 1 to 10 except even numbers
   ANSWER:
   i=0
for i in range(11):
  if(i%2==0):
    i=i+1
  else:
    product=i*i
    print(product)
    i=i+1
3. Your monthly expense list (from Jan to May) looks like this,
```
expense_list = [2340, 2500, 2100, 3100, 2980]
```
Write a program that asks you to enter an expense amount and program
should tell you in which month that expense occurred. If expense is not
found then it should print that as well.
ANSWER:
expense ={
      2340 : "January",
      2500 : "February",
      2100 : "March",
      3100 : "April",
      2980 : "May"
}
n=int(input("enter the number"))
j=0
for i in expense:
  if(i==n):
   print("expense found"+expense[i])
   j=j+1
   break
  elif(i!=n and j==len(expense)-1):
    print("expense not found")
    j=j+1
  else:
    j=j+1


4. Lets say you are running a 5 km race. Write a program that,
   1. Upon completing each 1 km asks you "are you tired?"
   2. If you reply "yes" then it should break and print "you didn't finish the race"
   3. If you reply "no" then it should continue and ask "are you tired" on every km
   4. If you finish all 5 km then it should print congratulations message

ANSWER:
  for i in range(5):
  j=0
  n=input("are you tierd?")
  if(n=="yes"):
      print("But you did not finish the race")
      j=j+1
      break;
  elif(n=="no"):
        j=j+1

  if(i==4):
    print("you completed the 5km run")


5. Write a program that prints following shape
```
*
**
***
****
*****
```
ANSWER
for i in range(1, 6):
  print("*" * i)

  


[Solution](https://github.com/codebasics/py/blob/master/Basics/Exercise/9_for/9_for_exercise.py)
