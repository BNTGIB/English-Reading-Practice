# [Human readable duration format]

- **Link:** : https://www.codewars.com/kata/58905bfa1decb981da00009e
- **Difficulty:** 3 Kyu
- **Date:** 29/04/2026

## 1. New Vocabulary


## 2. Approach & Logic 
- Iterate through the "floor" (`tmp[i]`), get all people who need to go up, also let the people out when reach their direction. Any time the lift reach the floor that HAS people want to go up, open the door even the lift is full. At the end of "up", change the value of `top` to the last floor that `open=1`.
- Similar with "down", start at `top` (the last floor that door open).
- Rule: anytime the lift open(stop), if that floor is not the same as the floor at last time the Lift stopped, add it to `vector<int> result`. We get the list of all floors that the Lift stopped with order visited.