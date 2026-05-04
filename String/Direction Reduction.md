# [Directions Reduction]

- **Link:** 
- **Difficulty:** 5 kyu
- **Date:** 04/05/2026

## 1. New Vocabulary
- **Dreadful weather**: thời tiết tồi tệ

## 2. Approach & Logic 
- The rule: `"NORTH" and "SOUTH" are opposite, "WEST" and "EAST" too.`
- Create `vector<string> result` to contain the result array of strings.
- Interate through the array of strings (`vect<string> arr`). If the present string is opposite with the last string of `result`, removed the that last string. If not, add the present string to `result`.
- Anyway, if the `result` is empty, that mean we dont have "the last string" to check, so we just add the present string to `result`.