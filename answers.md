# CMPS 2200 Assignment 5
## Answers

**Name:** Reagan Esteves


Place all written answers from `assignment-05.md` here for easier grading.





- **1a.**
 This algorithm is a greedy algorithm  that is used to pick the largest Geometrica denomination available. The cycle drops from lower and lower through each denomination until it cannot no more,the cycle will proceed until it has the desired amount of change it needs. The largest denomination is always apart of the set so it produces few coins making it an optimal algorithm
- **1b.**
 Work is O(log_2(n))
  Span is O(log_2(n))
- **2a.**

A counter example is with the denominations {1,5,6,9}, it is optimal to get 11 through 5 and 6. with 2 coins, but a greedy algorithm would choose 9, and 1 twice. This would lead to the greedy algorithms return 3 coins instead of 2. So in this case, the greedy can't work optimally. 



- **2b.**

If there are c number of coins then:
Work is O(n*c)
Span is O(n*c)


- **3a.**
The optimal substructre property for this verison of the edit distance is
first when  S[0] = T[0], then MED(S[1:], T[1:]) then when S[0] does not equal T[0], then 1 + min(MED(S, T[1:]), MED(S[1:], T), MED(S[1:],T[1:]))