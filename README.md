# Basic-Phy
Basic programming/Phyton exercises

Exercise 11

Ask the user for a number and determine whether the number is prime or not. (For those who have forgotten, a prime number is a number that has no divisors.). You can (and should!) use your answer to Exercise 4 to help you.

num= int(input('Please tell me your number: '))

div = [elem for elem in list(range(2,num)) if num%elem==0]

if len(div) ==0:
    print ('Is prime')
else: 
    print ('No prime')


Exercise 12 (and Solution)

Write a program that takes a list of numbers (for example, a = [5, 10, 15, 20, 25]) and makes a new list of only the first and last elements of the given list. For practice, write this code inside a function.

list = [5, 10, 15, 20, 25]
def first_last(list):
    return [list[0], a[list(a)-1]]


Exercise 14 (and Solution)

Write a program (function!) that takes a list and returns a new list that contains all the elements of the first list minus all the duplicates.

import random
a = random.sample(range(1,15), 10)
b = random.sample(range(1,20), 12)
list_c=[]
print([elem for elem in a if elem in b and elem not in list_c ])

***

import random
a = random.sample(range(1,15), 10)
b = random.sample(range(1,20), 12)
def list_unique (x,y):
    list_c=[]
    for el in a:
        if el in b and el not in list_c:
            list_c.append(el)
    return print(list_c)

list_unique (a,b)

print (a)
print (b)

***

a=[1,1,2]
set(a)
for elem in set(a):
    a_unique.append(elem)
print (a_unique)
