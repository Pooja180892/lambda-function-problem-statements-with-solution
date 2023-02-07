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
