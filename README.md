# Day-1 (part2)

def isPalindrome(N):
    original_num = N  
    reversed_num = 0  # we took it zero because it will act as a starting point,We start with reversed_num = 0 because we haven’t added any digits yet.
    while N > 0:
        last_digit = N % 10 
        reversed_num = reversed_num * 10 + last_digit  
        N = N // 10  
    return original_num == reversed_num
