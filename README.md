# Blind-leetcode soulutions
In this Article we will solve leetcode blind questions (https://leetcode.com/discuss/general-discussion/460599/blind-75-leetcode-questions) topicwise.
All the code that I will write below will be maintained in repo :-  https://github.com/amanlalwani007/blind-leetcode , so you can download the code in your local .
****

## Arrays
### Quo 1 :- Two Sum(https://leetcode.com/problems/two-sum/)

Problem statement :- Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

Sample testcase:- 
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

Solution :- 

```
Approach 1(Native or Brute Force):- 
Run a loop and compare every combination weather their sum matches to target if matched then return indeixes else return -1
Algo:- 
for i=0 to len(arr):
    for j=i+1 to len(arr):
        if arr[i]+arr[j]==target:
            return [i,j]
return -1              

Time Complexity :- O(N**2)
Space complexity :- O(1)

Approach 2 (using map):- 
Loop through all values in array if target-current_value found in map then return i ,map[target-current_value] else add value in map map[current_value]=index of current_value

Code :- 

```







