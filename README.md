# Basic-Calculator
user_name = input("Greetings!! What is your name: ")

#Write the same greeting above with the user’s name
print("Hello, "+ user_name +" ! This is now offcially your calculator!")
# Program to create a basic calculator called the JP-83 Silver Edition

# This operation adds two values
def add(x,y):
    return x + y

# This operation will subtract two values
def subtract(x,y):
    return x - y

# This operation multiplies two values
def multiply (x,y):
    return x*y

# This operation divides two values
def divide(x,y):
    return x/y

print("select an operation")
print("1.Add")
print("2.Subract")
print("3.Multiply")
print("4.Divide")

#Select an Operation
choice = input("Enter Operation Choice (1/2/3/4) ")

#Verify that user selected valid choice
if choice in ('1','2','3','4'):
    num1= float(input("Enter first number: "))
    num2= float(input("Enter Second number: "))
    if choice == '1':      
        print(num1,'+',num2, "=", add(num1,num2))
    elif choice == '2':
        print(num1,'-',num2,'=', subtract(num1,num2))
    elif choice == '3':
        print(num1, '*',num2, '=', multiply(num1,num2))
    elif choice == '4':
        print(num1, '/',num2, '=', divide(num1,num2))
    
    else: print("ERROR")
