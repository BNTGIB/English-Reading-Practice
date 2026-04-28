# [Large Factorials]

- **Link:**:  https://www.codewars.com/kata/557f6437bf8dcdd135000010
- **Difficulty:** 4 Kyu
- **Date:** 28/05/2026

## 1. New Vocabulary
- **mathematic** (n): Toán học
- **factorial** (n): Giai thừa
- **product of two numbers** (n): tích của hai số

## 2. Approach & Logic 
- I program a `mul(string a, int)` function to calculate the product of `string a` and `int b` with Vietnamese Multiplication Method (https://kuliso.org/learn/multiplication-in-vietnamese).
- Iterate through string `a` from the last element to the first. For each, multiply it with b, add with `boost`(`boost=0` for first loop), and we have `value`. Push the units digit of `value` to `string result`, also change `boost=value/10`.
- In next loop, `value` will be product of `a[i]` and `b`, and adding `boost`.
- After the loop terminates, reverse `to_string(boost)` and add it to result, and we have the string that contain the product of `string a` and `int b` BUT in reverse write order. So we ` reverse(res.begin(), res.end())` to get the correct result.
- In `factorial(int factorial)` funtion, I calculate the factorial of `factorial` with the base rule, using `mul()` to multiply.