# Palindrome-Number

class Solution:
    def isPalindrome(self, x):
        if x < 0:
            return False

        original_x = x
        reversed_x = 0

        while x > 0:
            digit = x % 10
            reversed_x = reversed_x * 10 + digit
            x //= 10

        return original_x == reversed_x


solution_instance = Solution()


print(solution_instance.isPalindrome(121))   
print(solution_instance.isPalindrome(-121))  
print(solution_instance.isPalindrome(10))   
