# Blind-leetcode soulutions
In this Article we will solve leetcode blind questions (https://leetcode.com/discuss/general-discussion/460599/blind-75-leetcode-questions) topicwise.
All the code that I will write below will be maintained in repo :-  https://github.com/amanlalwani007/blind-leetcode , so you can download the code in your local .
****

## Arrays
### Quo 1 :- Two Sum(https://leetcode.com/problems/two-sum/)

Problem statement :- Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

Sample testcase:- 
```
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
```
Solution :- 

```
Approach 1(Native or Brute Force):- 
Run a loop and compare every combination weather their sum matches to target if matched then return indeixes else return -1
Algo:- 
for i=0 to len(arr)-1:
    for j=i+1 to len(arr)-1:
        if arr[i]+arr[j]==target:
            return [i,j]
return -1              

Time Complexity :- O(N**2)
Space complexity :- O(1)

Approach 2 (using map):- 
Loop through all values in array if target-current_value found in map then return i ,map[target-current_value] else add value in map map[current_value]=index of current_value.

Time Complexity :- O(N)
Space complexity :- O(N)
```
Approach 2 Code :- https://github.com/amanlalwani007/blind-leetcode/blob/main/1.Two_Sum.java


### Quo 2 :- Best Time to Buy and Sell Stock (https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)

Problem Statement :-  You are given an array prices where prices[i] is the price of a given stock on the ith day.
You want to maximize your profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock.
Return the maximum profit you can achieve from this transaction. If you cannot achieve any profit, return 0.

Sample TestCase:- 

```
Input: prices = [7,1,5,3,6,4]
Output: 5
Explanation: Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = 6-1 = 5.
Note that buying on day 2 and selling on day 1 is not allowed because you must buy before you sell.
```
Solution :- 

```
Approach 1(brute force approach):-
Run two loop and try to buy stock everday and sell it on every day afterwards and calculate max profit 
Algo :- 
profit=0
for i 0 to len(arr)-2:
    for j i+1 to len(arr)-1:
        profit =max(profit, arr[j]-arr[i])
return profit 

Time Complexity :- O(N**2)
Space complexity :- O(1)

Approach 2 (optimized approach):- 
In this while traversing we maintain min_stock_price_till_now and sell stock everyday 
and calculate max_profit. 

```
Approach 2 Code :- 



