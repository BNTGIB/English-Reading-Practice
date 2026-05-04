# [Range Extraction]

- **Link:** https://www.codewars.com/kata/51ba717bb08c1cd60f00002f
- **Difficulty:** 4kyu
- **Date:** 04/05/2026

## 1. New Vocabulary
- **denoted** (v): được biểu thị
- **interval** (v): khoảng
- **Traverse the array** (v) :Duyệt qua mảng


## 2. Approach & Logic
- Tracking sequences: traverse the array and compare the current element with the previous one. If the difference is 1, I increment the counter `cs`.
- Handling breaks: When the sequence breaks (difference `>=2`), I check the counter. If `cs >= 3`, I format it as a range (`e.g., 1-5`). Otherwise, I list the numbers individually separated by commas.
- Edge case (The end of array): I added a specific check for the last element to ensure that any ongoing sequence is properly appended to the result string before the function returns.