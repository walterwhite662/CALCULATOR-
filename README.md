# CALCULATOR-
#IT IS A SIMPLE CALCULATOR THAT PERFORM ARITHMETIC OPERATION 
#ADDITION 
#SUBTRACTION
#MULTIPLICATION
#DIVISION


def add(x,y):
    return x + y
def sub(x,y):
    return x - y
def multi(x,y):
    return x * y
def divide(x,y):
    return x/y
print("select operation.")
print("1.add")
print("2.sub")
print("3.multi")
print("4.divide")
while True:
    choice = input("enter choice(1/2/3/4):")
    if choice in('1','2','3','4'):
        try:
            num1=float(input("enter number"))
            num2=float(input("enter number"))
        except ValueError:
            print("invalid input")
            continue
        if choice == '1':
            print(num1,"+",num2,"=",add(num1,num2))
        elif choice =='2':
            print(num1,"-",num2,"=",sub(num1,num2))
        elif choice =='3':
            print(num1,'*',num2,"=",multi(num1,num2))
        elif choice == '4':
            print(num1,"/",num2,"=",divide(num1,num2))
        next_calculation = input("new calculation")
        if next_calculation =="no":
            break
        else:
            print("invalid Input")
            

    

