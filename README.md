# Leetcode-242.-Valid-Anagram
# Description
Given two strings s and t, return true if t is an anagram of s, and false otherwise.
# Solution
An anagram is a word or phrase formed by rearranging the letters of a different word or phrase, using all the original letters exactly once.

Example 1:

Input: s = "anagram", t = "nagaram"

Explanation: s has 3 a's , 1 n , 1 m , 1 g . 

In a similar way string t has 3 a's , 1 n , 1 m , 1 g  .

Hence True

Output: true

Example 2:

Input: s = "rat", t = "car"

Explanation: string s has 1 r,1 a , 1 t .

String t has 1 c , 1 a , 1 r

Hence false

Output: false
# Algorithm
1. Sort the strings s and t alphabetically.
2. And comapre whether they are equal or not.
3. If they are equal return true else return false.
# Code
class Solution:

    def isAnagram(self, s: str, t: str) -> bool:
        sorted_s=sorted(s)
        sorted_t=sorted(t)
        if sorted_s==sorted_t:
            return True
        return False
# Complexity
Time Complexity:

The sort operation takes O(1) time

The if comparison operation takes O(1) time

Hence : O(1) 

Space Complexity:

Variables like sorted_t and sorted_s are used to store the sorted strings which has memory space of O(1)
