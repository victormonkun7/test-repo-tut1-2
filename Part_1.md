# Exercise 1: Prime Number Checker  
- This code checks if a number entered by the user is prime or not.  
- It first ensures the input is an integer by comparing the `float` and `int` versions of the input.  
- If the number is a floating-point value, the program asks the user to enter a non-floating number.  
- It then checks for two conditions:  
  - If the number is `0` or odd, it prints:  
    **"This is not a prime number"**.  
  - Otherwise, it assumes the number is prime and prints:  
    **"This is a prime number"**.  

## Example Output  
- Enter a number: 7  
This is not a prime number  

- Enter a number: 4  
This is a prime number  

- Enter a number: 5.5  
Write a non-floating number!  


# Exercise 2: Fibonacci Sequence Generator  
- This code generates and displays a Fibonacci sequence based on the number of terms entered by the user.  
- It first asks the user how many Fibonacci numbers they want.  
- If the input is less than or equal to `0`, it displays:  
  **"The number couldn't be less than 1"**.  
- Otherwise, it:  
  - Initializes the sequence with the first two numbers: `0` and `1`.  
  - Uses a `for` loop to calculate and append the next numbers by summing the two previous ones.  
  - Prints the desired amount of the Fibonacci sequence.  

## Example Output  
 - Please enter how many numbers you want in Fibonacci set to be calculated and displayed: 5
Fibonacci sequence: 0 1 1 2 3

- lease enter how many numbers you want in Fibonacci set to be calculated and displayed: 1
Fibonacci sequence: 0

- Please enter how many numbers you want in Fibonacci set to be calculated and displayed: 0
The number couldn't be less than 1


# Exercise 3: Star Pattern Generator  
- This code generates a **right-angled inverted triangle** pattern using stars (`*`).  
- It defines the number of rows (`n = 5`).  
- The **outer loop** iterates over each row (`i` ranges from `0` to `n-1`).  
- The **inner loop** controls the number of stars printed in each row:  
  - It starts from `i` and goes up to `n`, decreasing the number of stars with each row.  
- A newline is printed after each row to move to the next line.  

## Example Output  
\* \* \* \* \*  
\* \* \* \*  
\* \* \*  
\* \*   
\*  


# Exercise 4: String Reversal  
- This code reverses a string entered by the user.  
- It defines a function `reverse_string()` that:  
  - Takes input from the user.  
  - Prints the reversed string using slicing (`[::-1]`).  
- The function is then called to execute the program.  

## Example Output  
- Enter a string: hello  
Reversed string: olleh

- Enter a string: Python  
Reversed string: nohtyP


# Exercise 5: Min and Max Finder  
- This code defines a function `min_max()` that finds the **minimum** and **maximum** values in an iterable (e.g., list, tuple).  
- It uses the `min()` and `max()` functions to extract the smallest and largest values, respectively.  
- The function returns the values as a **tuple**.  
- The program then demonstrates the function by calling it with a list of numbers, unpacking the result, and printing the min and max values.  

## Key Explanation:  
### `return min(numbers), max(numbers)`
- This line returns **two values** from the function:  
  - `min(numbers)` → The smallest value in the iterable.  
  - `max(numbers)` → The largest value in the iterable.  
- Since the function returns two values separated by a comma, they are automatically packed into a **tuple**.  
- For example:  
  ```python
  values = [5, 12, 3, 9, 18]  
  result = min_max(values)  
  print(result)  # Output: (3, 18)  

## Example Output 
Min value is: 3  
Max value is: 18


# Exercise 6: Random Number Guessing Game  
- This program generates a **random number** between `1` and `10` and lets the user guess it.  
- It uses a **while loop** to keep the game running until the user guesses correctly.  
- The program provides feedback on whether the guess is **too low**, **too high**, or **correct**.  

## Key Explanation:  
### `import random`
- The `random` module in Python is used to **generate random numbers**.  
- `import random` gives access to all the functions in the `random` module.  
- In this program, the function `random.randint(1, 10)` generates a random integer between `1` and `10` (inclusive).  
- Example:  
  ```python
  random_number = random.randint(1, 10)  
  print(random_number)  # Could print any number between 1 and 10  
