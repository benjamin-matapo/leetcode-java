# 412. Fizz Buzz

---

## Problem

Given an integer `n`, return a string array answer (1-indexed) where:

`answer[i] == "FizzBuzz"` if `i` is divisible by `3` and `5`.
`answer[i] == "Fizz"` if `i` is divisible by `3`.
`answer[i] == "Buzz"` if `i` is divisible by `5`.
`answer[i] == i` (as a string) if none of the above conditions are true.


Example 1:

`Input: n = 3`
`Output: ["1","2","Fizz"]`

Example 2:

`Input: n = 5`
`Output: ["1","2","Fizz","4","Buzz"]`

Example 3:

`Input: n = 15`
`Output: ["1","2","Fizz","4","Buzz","Fizz","7","8","Fizz","Buzz","11","Fizz","13","14","FizzBuzz"]`


Constraints:

`1 <= n <= 10^4`

---

# Approach

* Made a for loop that loops through each character in the array
* Outputs "FizzBuzz" if `i % 15 == 0` (If `i` is perfectly divisible by 3 and 5)
* Outputs "Fizz" if `i % 3 == 0`
* Outputs "Buzz" if `i % 5 == 0`

---

# Complexity

Big O notation is a paradigm used to quantify hoe efficient an array is, specifically how it behaves at the input gets bigger

* *O(n)* means that the time it takes grows *linearly*, i.e. if `n = 15`, it does 15 steps, and if `n = 100`, it does 100 steps
* *O(1)* means that it takes the same amount of time regardless of the input, e.g. `return "hello"`, doesn't matter if n = 5 or 5 million, it's one instant operation

* **Time:** This is how long it takes to run. It uses *O(n)*, taking `n` time units linearly to run
* **Space:** This is how much memory it uses. It uses *O(n)* as well, so it takes up `n` amount of items in the list

---

## Notes

* It is more concise to check for divisibility of i by 15 for the "FizzBuzz" condition, as all numbers that are divisible by both 3 and 5 will be divisible by 15