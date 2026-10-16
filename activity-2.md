# Activity 2: Logic Building Challenge 
Students solve progressively complex logical problems using flowcharts and pseudocode before implementing them in code.
#
# Activity 2: Logic Building Challenge

## 1. Aim

To develop logical thinking and problem-solving skills by solving programming problems using algorithms, flowcharts, pseudocode, and Python programming.

## 2. Introduction

Logic building is the process of analyzing a problem and developing a sequence of steps to solve it. Flowcharts visually represent these steps, while pseudocode describes the solution in a simple, programming-like format before implementation.

## 3. Problem 1: Check Whether a Number Is Even or Odd

### Algorithm

1. Start.
2. Read an integer `n`.
3. Check whether `n % 2 == 0`.
4. If true, display "Even Number".
5. Otherwise, display "Odd Number".
6. Stop.

### Flowchart

```text
       +-----------+
       |   START   |
       +-----------+
             |
             v
       / Input n  /
      +-----------+
             |
             v
       < n % 2 == 0? >
          /       \
        Yes        No
         |          |
         v          v
  +------------+ +------------+
  | Print Even | |  Print Odd |
  +------------+ +------------+
         \          /
          v        v
       +-----------+
       |    END    |
       +-----------+
```

### Pseudocode

```text
START
INPUT n
IF n MOD 2 = 0 THEN
    PRINT "Even Number"
ELSE
    PRINT "Odd Number"
END IF
STOP
```

### Python Code

```python
n = int(input("Enter a number: "))

if n % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")
```

### Sample Output

```text
Enter a number: 8
Even Number
```

## 4. Problem 2: Find the Largest of Three Numbers

### Algorithm

1. Start.
2. Read three numbers `a`, `b`, and `c`.
3. Compare the numbers.
4. If `a` is greater than or equal to both `b` and `c`, print `a`.
5. Otherwise, if `b` is greater than or equal to both `a` and `c`, print `b`.
6. Otherwise, print `c`.
7. Stop.

### Pseudocode

```text
START
INPUT a, b, c
IF a >= b AND a >= c THEN
    PRINT a, "is the largest"
ELSE IF b >= a AND b >= c THEN
    PRINT b, "is the largest"
ELSE
    PRINT c, "is the largest"
END IF
STOP
```

### Python Code

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))

if a >= b and a >= c:
    print(a, "is the largest")
elif b >= a and b >= c:
    print(b, "is the largest")
else:
    print(c, "is the largest")
```

### Sample Output

```text
Enter first number: 12
Enter second number: 25
Enter third number: 18
25 is the largest
```

## 5. Problem 3: Calculate the Factorial of a Number

### Algorithm

1. Start.
2. Read a non-negative integer `n`.
3. Initialize `factorial = 1`.
4. Multiply `factorial` by every integer from 1 to `n`.
5. Display the factorial.
6. Stop.

### Pseudocode

```text
START
INPUT n
IF n < 0 THEN
    PRINT "Enter a non-negative number"
ELSE
    factorial = 1
    FOR i = 1 TO n
        factorial = factorial * i
    END FOR
    PRINT factorial
END IF
STOP
```

### Python Code

```python
n = int(input("Enter a non-negative integer: "))

if n < 0:
    print("Enter a non-negative number")
else:
    factorial = 1

    for i in range(1, n + 1):
        factorial *= i

    print("Factorial =", factorial)
```

### Sample Output

```text
Enter a non-negative integer: 5
Factorial = 120
```

## 6. Explanation

- **Algorithm:** Provides step-by-step instructions to solve a problem.
- **Flowchart:** Represents the steps and decisions using standard symbols and arrows.
- **Pseudocode:** Describes the logic in simple, structured language.
- **Python program:** Implements the logic so the computer can execute it.

These techniques help identify errors and organize the solution before writing a complete program.

## 7. Result

Successfully solved logical problems using algorithms, flowcharts, pseudocode, and Python programming. Improved problem-solving skills and understanding of conditional statements and loops.
