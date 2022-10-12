#Question 1:
# Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
# You may assume that each input would have exactly one solution, and you may not use the same element twice.
# You can return the answer in any order. 
#Follow-up: Can you come up with an algorithm that is less than O(n2) time complexity?


#hint : to find 2 numbers of which sum = or != to a target numbr:
    #subtract both nums from target and check if 1st num=target-2nd numbr
    #if yes : result=true else: result=false
def twoSum(nums, target):    
    d = {}
    for i, item in enumerate(nums):
        res = target - item
        if res in d: return [d[res], i]
        d[item] = i
    
print(twoSum([2,51,8,11],10))





