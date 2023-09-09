# calculator

def add(a , b):
    return (a + b)

def subtract(a , b):
    return a - b 


def multiply(a , b):
    return(a * b)

def divide(a ,b):
    if b != 0:
        return (a / b) 
    else:
        return ("Din't divided by 0")

print("Select arithmetic operations :")
print("1. add\n2. subtract\n3. multiply\n4. divide")


operation_choice = input("Please enter your choice (1/2/3/4): ")


num1 = float(input("Please enter first number : "))
num2 = float(input("Please enter second number : "))

if operation_choice == '1':
    print(num1,"+",num2,"=",add(num1 , num2),"\nAddition of two numbers is done....\nThanks....")
elif operation_choice == '2':
    print(num1,"-",num2,"=",subtract(num1 ,num2),"\nSubstraction of two numbers is done....\nThanks....")
elif operation_choice == '3':
    print(num1,"*",num2,multiply,"=",multiply(num1 , num2),"\nMultiplication of two numbers is done....\nThanks....")
elif operation_choice == '4':
    print(num1,"/",num2,"=",divide(num1 , num2),"\nDivision of two numbers is done....\nThanks....")
else:
    print("Your input is Invalid....\nPlease enter valid input....")

