# code1
def is_armstrong_number(number):
    # Convert the number to a string to count digits
    num_str = str(number)
    # Calculate the number of digits
    num_digits = len(num_str)
    
    # Calculate the sum of each digit raised to the power of the number of digits
    armstrong_sum = sum(int(digit) ** num_digits for digit in num_str)
    
    # Check if the sum equals the original number
    return armstrong_sum == number

# Input number to check
num = int(input("Enter a number to check for Armstrong: "))

# Check if the number is an Armstrong number
if is_armstrong_number(num):
    print(f"{num} is an Armstrong number")
else:
    print(f"{num} is not an Armstrong number")
