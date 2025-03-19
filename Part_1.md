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

## Example Output
- Guess the number (1-10): 4  
Too low! Try again.  

- Guess the number (1-10): 10  
Too high! Try again.  

- Guess the number (1-10): 8  
🎉 Correct! You win!  


# Exercise 7: Password Checker  
- This program continuously prompts the user to enter a password until the correct one is provided.  
- It uses a **while loop** to keep asking for the password until the correct one is entered.  
- The program checks if the password matches the predefined value (`"Python123"`) and grants access when it does.  

## Example Output  
Enter the password: hello  
Incorrect password. Try again.

Enter the password: Python123  
Access Granted!


# Exercise 8: Series Calculation  
- This program calculates the series:  
  \[ x \times \frac{5^{2}}{1 + 2!} + x \times \frac{25^{2}}{2 + 3!} + ... \text{(N terms)} \]  
- It uses the `math` module for the **factorial** function.  
- The program:  
  - Takes input values for `x` and `N`.  
  - Defines the function `calculate_series(x, N)` to compute the series.  
  - Iterates over `N` terms and accumulates the total.  
- Finally, it displays the result.  

## Why Use the `math` Module?  
- The `math` module provides efficient mathematical operations, including the **factorial operator**.  
- `math.factorial(n)` returns the factorial of `n` (e.g., `math.factorial(3)` → `6`).  
- Using the module simplifies the calculation, making the code cleaner and more efficient.  

## Example Output  
- Enter the value of x: 2
- Enter the number of terms (N): 3  
Series result: 10.482142857142858


# Exercise 9: Mirror Reflection of an Image  
This program:  
- Loads an image from an online URL.  
- Converts it into a **NumPy array**.  
- Generates **horizontal** and **vertical** mirror reflections.  
- Displays the original and mirrored images using **Matplotlib**.  

---

## ✅ **Explanation**
1. **Modules used:**  
   - `requests`: Downloads the image from a URL.  
   - `Pillow (PIL)`: Opens and processes the image.  
   - `NumPy`: Converts the image into an array and creates mirrored reflections.  
   - `Matplotlib`: Displays the original and mirrored images.  

2. **Code validation tools:**  
   - `try-except` blocks → Catch and handle errors gracefully.  
   - `response.raise_for_status()` → Verifies that the image request is successful.  
   - Image validation → Ensures the image loads correctly before processing.  

---

## 🚀 **Sample Output**
- **Original Image**  
- **Horizontal Mirror Reflection**  
- **Vertical Mirror Reflection**


# Exercise 10: Temperature Data Analysis  
This program:  
1. Creates a **NumPy array** with temperature data.  
2. Finds the **minimum**, **maximum**, and **average** temperatures.  
3. Converts the temperatures from **Celsius to Fahrenheit**.  
4. Identifies all days where the temperature was **above 25°C**.  
5. Counts how many days had temperatures **below 20°C**.  
6. Sorts the temperature data in **ascending order**.  
7. Reshapes the 1D array into a **5x6 2D array** representing weeks (5 weeks of 6 days each).  

---

## ✅ **Explanation**
1. **Modules used:**  
   - `numpy`: Library for numerical operations and array manipulations.  

2. **Key operations performed:**  
   - **Temperature analysis:** Min, max, and average values are calculated.  
   - **Fahrenheit conversion:** Uses the formula:  
     \[ F = C \times \frac{9}{5} + 32 \]  
   - **Filtering:** Finds all days with temperatures over 25°C.  
   - **Counting:** Counts how many days were below 20°C.  
   - **Sorting:** Sorts the temperatures in ascending order.  
   - **Reshaping:** Creates a 2D array of 5 weeks with 6 days each.  

---

## 🚀 **Sample Output**
Min: 18  
Max: 30  
Average: 23.1  

Fahrenheit: 71.6, 75.2, 66.2, 69.8, 73.4, 77.0, 78.8, 80.6, 75.2, 73.4, 68.0, 71.6, 69.8, 66.2, 64.4, 71.6, 73.4, 75.2, 78.8, 82.4, 86.0, 80.6, 77.0, 78.8, 75.2, 71.6, 69.8, 68.0, 66.2, 73.4

Above 25°C: 26, 27, 26, 28, 30, 27, 26

Days below 20°C: 4

Sorted Temps: 18, 19, 19, 19, 20, 20, 21, 21, 21, 22, 22, 22, 22, 23, 23, 23, 23, 24, 24, 24, 24, 25, 25, 26, 26, 26, 27, 27, 28, 30

5x6 Array (Weeks):  
[[22 24 19 21 23 25]  
[26 27 24 23 20 22]  
[21 19 18 22 23 24]  
[26 28 30 27 25 26]  
[24 22 21 20 19 23]]  