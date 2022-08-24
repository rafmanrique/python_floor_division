# What Does // Mean in Python?

The double slash `//` operator in Python is used to divide a number by its floor. The first number is divided by the second number using the `//` operator, and the result is rounded to the nearest integer (or whole number). Floor division merely differs from ordinary division in that it always produces the largest integer.

<p align="center">
  <img src="https://i.ytimg.com/vi/mv5uHSXLkhs/maxresdefault.jpg" width='450px'/>
</p>

## What Does // Mean in Python? Points of Interest

 - [Syntax of the Floor Division](#syntax)
	 - Regular Division vs Floor Division (/ vs //)
- [Working with Negative Numbers in Floor Divisions](#negative)

## Syntax of the Floor Division <a name="syntax"></a>
```

The syntax for using the floor division is given as follows:
```py
quotient = divident // divisor
```
The double slash `//` operator is used in almost identical ways to ordinary division. The only difference is that you use a double slash `//` rather than a single slash `/`.

### Regular Division vs Floor Division (/ vs //)

The result of regular division (using the `/` operator) is `45/6=7.5`, but using `//` has floored `7.5` down to `7`.

If one of the operands is a float in floor division, the output will also be a float, whereas the result of ordinary division is always a float.

The following is an illustration of this:

```py
num1 = 19
num2 = 5
num3 = num1 / num2
num4 = num1 // num2

print("normal division of", num1, "by", num2, "=", num3)
print("floor division of", num1, "by", num2, "=", num4)
# Output: 
# normal division of 19 by 5 = 3.8
# floor division of 19 by 5 = 3
```

## Working with Negative Numbers in Floor Divisions <a name="negative"></a>
When the operand is negative, the largest integer that is less than or equal to the outcome of ordinary division will be returned by floor division. To demonstrate how this operates, let's use the same operands as before:

```py
num1 = 19
num2 = 5
num3 = -19
num4 = num1 / num2
num5 = num1 // num2
num6 = num3 // num2

print("normal division of", num1, "by", num2, "=", num4)
print("floor division of", num1, "by", num2, "=", num5)
print("floor division of", num3, "by", num2, "=", num6)
# Output: 
# normal division of 19 by 5 = 3.8
# floor division of 19 by 5 = 3
# floor division of -19 by 5 = -4
```
