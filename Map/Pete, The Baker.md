# [Pete, The Baker]

- **Link:** https://www.codewars.com/kata/525c65e51bf619685c000059
- **Difficulty:** 5 kyu
- **Date:** 06/05/2026

## 1. New Vocabulary
- **bake** (n): nướng (bánh)


## 2. Approach & Logic (Giải thích logic bằng tiếng Anh)
- Loop through `recipe` with `for(auto [ingre,units] : recipe)`, if `units` is equal to `0`, that's mean we don need that Ingredient for cake, so we skip it.
- If not, we check if the `available` ingredients is enough for that ingredient and `return 0` if is not enough.
- Then, calculate the `possibale` numbers of cake can be baked with that available ingredients, update `res` if that `possible` was the minimum. Then return `res`, which was the number of cake that can be baked.