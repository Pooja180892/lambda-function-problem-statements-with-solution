# lambda-function-problem-statements-with-solution
lambda function problem statements with solution
Write a Python program to create a lambda function that adds 15 to a given number passed in as an argument, also create a lambda function that multiplies argument x with argument y and print the result.M
val = lambda x : x + 15
print(val(15))
val = lambda x, y : x * y
print(val(12, 4))

Write a Python program to create a function that takes one argument, and that argument will be multiplied with an unknown given number.
n=int(input('enter the no.:'))
a=lambda x:x*float(input('enter a number'))
print(a(10))

#3.Write a Python program to sort a list of tuples using Lambda.
l=[('English', 88), ('Science', 90), ('Maths', 97), ('Social sciences', 82)]
res=lambda x:sorted(x)
print(res(l))
print(sorted(l,key=lambda x:x[1]))

Write a Python program to sort a list of dictionaries using Lambda.
dict=[{'make': 'Nokia', 'model': 216, 'color': 'Black'}, {'make': 'Mi Max', 'model': '2', 'color': 'Gold'}, {'make': 'Samsung', 'model': 7, 'color': 'Blue'}]
print(sorted(dict,key= lambda x:x['color']))

Write a Python program to square and cube every number in a given list of integers using Lambda.
num=int(input('enter the no.'))
res= lambda x:x**2
val=lambda x:x**3
print('square no.',res(num))
print('cube no.',val(num))

Write a Python program to find if a given string starts with a given character using Lambda.
s=input('enter the string')
res=lambda x:x.startswith('p')
print(res(s))

Write a Python program to extract year, month, date and time using Lambda.
import datetime
now = datetime.datetime.now()
print(now)
year = lambda x: x.year
month = lambda x: x.month
day = lambda x: x.day
t = lambda x: x.time()
print(year(now))
print(month(now))
print(day(now))
print(t(now))

Write a Python program to check whether a given string is number or not using Lambda.
s=input('enter the string')
res=lambda x:'is num' if x.isdigit() else 'not num'
print(res(s))

Write a Python program to find intersection of two given arrays using Lambda.
l1=[1,2,3,4]
l2=[2,3,4,5]
res = lambda x:x in l1
print(list(filter(res,l2)))

Write a Python program to rearrange positive and negative numbers in a given array using Lambda.
l1=[3,-1,5,6,-3,1,2]
res=list(filter(lambda x:x>0,l1))
res1=list(filter(lambda x:x<0,l1))
result=((sorted(res))+(sorted(res1)))
print(result)

13.Write a Python program to count the even, odd numbers in a given array of integers using Lambda.
l=[1,2,3,4,5,6,7,8,9]
print('even count', len(list(filter(lambda x:( x%2==0 ),l))))
print('odd count', len(list(filter(lambda x:( x%2!=0 ),l))))

Write a Python program to add two given lists using map and lambda.
l1=[1,2,3,4,5]
l2=[5,6,7,8,9]
res= lambda x,y:x+y
print(list(map(res,l1,l2)))
