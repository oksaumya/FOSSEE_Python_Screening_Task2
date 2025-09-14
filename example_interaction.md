# Example Interaction Demonstration

This file demonstrates how the AI debugging assistant prompt works in practice with different types of common Python bugs.

## Example 1: Logic Error (Beginner Level)

**Student Code:**
```python
def is_even(number):
    if number % 2 = 0:
        return True
    else:
        return False

print(is_even(4))  # Should print True but gives error
```

**AI Response (following the prompt):**
"Great start with your function structure! I can see you understand the concept of using modulo to check for even numbers.

I notice something on line 2 that's causing a syntax error. Take a close look at your conditional statement - what's the difference between assigning a value to a variable and checking if two values are equal in Python?

Try running your code and reading the error message carefully. What does Python tell you about line 2? Once you spot the issue, test your function with a few different numbers to make sure it works as expected."

---

## Example 2: Logical Error (Intermediate Level)

**Student Code:**
```python
def find_maximum(numbers):
    max_num = 0
    for num in numbers:
        if num > max_num:
            max_num = num
    return max_num

# Test cases
print(find_maximum([1, 5, 3, 9, 2]))  # Works: prints 9
print(find_maximum([-5, -2, -8, -1]))  # Problem: prints 0
```

**AI Response (following the prompt):**
"Nice work on the loop structure and comparison logic! Your function works perfectly for the first test case.

I see you've noticed an issue with negative numbers. Let's think about your initialization on line 2 - what assumption are you making about the numbers in the list when you set `max_num = 0`?

Try tracing through your second test case step by step. What happens when all numbers in the list are smaller than your initial value? Can you think of a better way to initialize `max_num` that would work regardless of what numbers are in the list?"

---

## Example 3: Index Error (Advanced Beginner)

**Student Code:**
```python
def get_last_three(my_list):
    result = []
    for i in range(3):
        result.append(my_list[len(my_list) - 1 - i])
    return result

# Works fine
print(get_last_three([1, 2, 3, 4, 5]))  

# Crashes
print(get_last_three([1, 2]))  
```

**AI Response (following the prompt):**
"Excellent approach using indexing from the end of the list! Your logic for accessing elements backwards is spot-on, and it works great when the list is long enough.

The error occurs when your list is shorter than expected. Let's think about what happens in your loop - you're always trying to get 3 elements, but what if the list doesn't have 3 elements?

Try adding some print statements to see what index values you're trying to access in the failing case. What could you check before starting your loop, or how might you modify your range to handle lists of any size?"

---

## Key Observations

Notice how each response:

1. **Starts positively** - acknowledges what the student did well
2. **Identifies the problem area** without stating the exact fix
3. **Asks guiding questions** that lead toward the solution
4. **Suggests investigation techniques** (print statements, tracing, testing)
5. **Maintains an encouraging tone** throughout

The prompt successfully scales from basic syntax errors to more complex logical issues while maintaining the same supportive, discovery-oriented approach.
