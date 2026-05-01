# [Find the odd int]

- **Link:**:  https://www.codewars.com/kata/557f6437bf8dcdd135000010
- **Difficulty:** 6 Kyu
- **Date:** 1/05/2026

## 1. New Vocabulary
- **counter variable(n)**: Biến đếm

## 2. Approach & Logic 
- Create a copy vector `tmp(numbers)`, sort it from small to big. 
- Iterate through the vector, if the element is the same number as the previos element, `count++`. If not, check the `count` of previos number and return the number if `count` is odd. 
- If not again, so that `tmp[i-1]` is not the answer, we convert `count` to present number's counter variable by reset so value `1` and countinue the loop to check.
- If the loop is end and we still not get the answer, that mean the last number is the answer, so we `return tmp[i-1]`.