# CISC230 - Jada Rose

## factorial2.cpp

Input/parameter impacting calls: integer n
Explanation: Each call reduces n by 1 until n == 0 or 1.
Examples:
factorial(3) → calls for 3, 2, 1 → 3 calls
factorial(5) → calls for 5, 4, 3, 2, 1 → 5 calls
factorial(7) → calls for 7 down to 1 → 7 calls
General case: Number of recursive calls = n
## ireverse2.cpp

Input/parameter impacting calls: length of string n
Explanation: Each call processes one character and reduces length until string is empty.
Examples:
"ab" (length 2) → 2 recursive calls
"cat" (length 3) → 3 recursive calls
"hello" (length 5) → 5 recursive calls
General case: Number of recursive calls = n

## sreverse2.cpp

Input/parameter impacting calls: length of string n
Explanation: Each call strips off one character and recurses on the rest.
Examples:
"a" (length 1) → 1 call
"dog" (length 3) → 3 calls
"house" (length 5) → 5 calls
General case: Number of recursive calls = n

## permute.cpp

Input/parameter impacting calls: length of string n
Explanation: For each position, the function recursively permutes the remaining substring, creating a branching recursion tree.
Examples:
"ab" (length 2) → 2! = 2 permutations → ~3 calls
"abc" (length 3) → 3! = 6 permutations → ~9 calls
"abcd" (length 4) → 4! = 24 permutations → ~33 calls
General case: Number of recursive calls ≈ n!
## tower.cpp

Input/parameter impacting calls: number of disks n
Explanation: To move n disks, the function calls itself twice with n-1, plus one move.
Examples:
n = 2 → 3 moves (calls)
n = 3 → 7 moves (calls)
n = 4 → 15 moves (calls)
General case: Number of recursive calls = 2^n – 1

## fibonacci2.cpp (presented in video lesson)

Input/parameter impacting calls: integer n
Explanation: Function calls itself twice for each n > 1, leading to exponential growth.
Examples:
fib(3) → 5 calls
fib(4) → 9 calls
fib(5) → 15 calls
General case: Number of recursive calls ≈ 2^n
