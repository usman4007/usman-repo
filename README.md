# usman-repo
# Function to check if a number is prime
def is_prime(n):
    if n <= 1:  # Numbers less than or equal to 1 are not prime
        return False
    for i in range(2, int(n ** 0.5) + 1):  # Check divisibility up to the square root of n
        if n % i == 0:
            return False
    return True

# Input to get the range
start = int(input("Enter the starting number: "))
end = int(input("Enter the ending number: "))

# Loop through the range and print prime numbers
for num in range(start, end + 1):
    if is_prime(num):
        print(num, "is a prime number")


      
