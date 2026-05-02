# [Human readable duration format]

- **Link:** : https://www.codewars.com/kata/52742f58faf5485cae000b9a
- **Difficulty:** 4 Kyu
- **Date:** 27/04/2026

## 1. New Vocabulary
- **format** (v):  Định dạng
- **resulting expression** (n): biểu thức kết quả
- **component** (n): thành phần
- **units of time** (n): ĐƠN VỊ về thời gian
- **plural** (adj): Dạng Số Nhiều

## 2. Approach & Logic 
- I use 2 vector `unit` (string) and `value_sec`(int) to contain strings of "unit of time" and value for each units that converted to seconds. Also 1 queue `appear`(int) that contain the indices of elements int `unit` which appear.
- Iterate through the array. For each element `unit[i]`, calculate the `value = sec / value_sec[i]` to know that unit is appear. If `value` is more than `0`, push the index `i` to `appear`, also change the value of `value_sec=value` to use it in next loop. 
- Create `string result=""`. With the `index` in queue `appear`, using another loop to add the resulting expression to `result`. Finally return `result`.