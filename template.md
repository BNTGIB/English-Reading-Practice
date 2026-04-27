# [Two Sum]

- **Link:** 
- **Difficulty:** Easy / Medium / Hard
- **Date:** 27/04/2026

## 1. New Vocabulary
- **Indices** (n): Các chỉ số (số nhiều của index).
- **Assume** (v): Giả sử, cho rằng.
- **Exactly one solution** (pharse): Có chính xác một nghiệm/cách giải.

## 2. Approach & Logic (Giải thích logic bằng tiếng Anh)
*Ép bản thân viết 2-3 câu tiếng Anh mô tả cách giải:*
- I use a **Hash Map** to store the value and its index.
- Iterate through the array. For each element `nums[i]`, calculate the `complement = target - nums[i]`.
- If the `complement` exists in the map, return their indices.