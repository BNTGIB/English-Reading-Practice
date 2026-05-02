# [Snail]

- **Link:**:   https://www.codewars.com/kata/521c2db8ddc89b9b7a0000c1
- **Difficulty:** 4 Kyu
- **Date:** 2/05/2026

## 1. New Vocabulary
- **outermost elements(n)**: phần tử ngoài cùng

## 2. Approach & Logic 
- The order: Right -> Down -> Left -> Up.
- Use `i`(row) and `j`(colum) to iterate through the matrix with that order.

For example: with `Matrix 4x4`.
    - Right: take all element of the first row, `i` and `j` would be `[0][3]` at the end.
    - Down: up the `i` to `[1]`, take any element of last colums (`j`=`3`). In the end -> `[3][3]`.
    - Right: minus 1 unit of `j` (to `[2]`) take all element of the last row (`i`=`3`) with the reverse order (`j=[2]->[0]`). `i` and `j` would be `[3][0]` at the end.
    - Up: minus 1 unit of `i` (to `[2]`), take element in first colums EXPECT the first-row's element, reverse order (`i=[2]->[1]`).
    - After any steps, check if `result` have taked all matrix's elements.
    - After the circle, the matrix would be `matrix 2x2`, do the circle againt until `result` have taked all matrix's elements (`result.size()= 16 `).

