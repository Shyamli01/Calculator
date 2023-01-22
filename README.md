# Calculator that ends calculation
[Calculator that ends calculation.txt](https://github.com/Shyamli01/Calculator/files/10475376/Calculator.that.ends.calculation.txt)
#Calculator
from art import logo
#Add
def add(n1,n2):
  return n1+n2

#Subtract
def subt(n1,n2):
  return n1-n2

#Multiply
def mult(n1,n2):
  return n1*n2

#Divide
def div(n1,n2):
  return n1/n2

operations = {"+":add,"-":subt,"*":mult,"/":div }
print(logo)
num1 = float(input("What's the first number?:"))
for symbol in operations :
  print(symbol)
should_continue = True
      
while should_continue:
  operation_symbol = input("Pick an operation : ")
  num2 = float(input("What's the next number?:"))
      
  calculation_function = operations[operation_symbol]
  answer = calculation_function(num1, num2)
      
  print(f"{num1} {operation_symbol} {num2} = {answer}")
  if(input(f"Type 'y' to continue calculating with {answer}, or tpye 'n' to exit the calculation.: "))== "y":
    num1 = answer
  else:
    should_continue= False
    
        
#Calculator that continues calculation

[Calculator.txt](https://github.com/Shyamli01/Calculator/files/10475378/Calculator.txt)

#Calculator
from art import logo
#Add
def add(n1,n2):
  return n1+n2

#Subtract
def subt(n1,n2):
  return n1-n2

#Multiply
def mult(n1,n2):
  return n1*n2

#Divide
def div(n1,n2):
  return n1/n2

operations = {"+":add,"-":subt,"*":mult,"/":div }
def calculator():
  print (logo)
  num1 = float(input("What's the first number?:"))
  
  for symbol in operations :
    print(symbol)
  should_continue = True
  
  while should_continue:
    operation_symbol = input("Pick an operation : ")
    num2 = float(input("What's the next number?:"))
  
    calculation_function = operations[operation_symbol]
    answer = calculation_function(num1, num2)
  
    print(f"{num1} {operation_symbol} {num2} = {answer}")
    if(input(f"Type 'y' to continue calculating with {answer}, or tpye 'n' to start a new calculation.: "))== "y":
      num1 = answer
    else:
      should_continue= False
      calculator()

calculator()
