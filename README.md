# project-euler-004
# largest palindrome product

"""
A palindromic number reads the same both ways. The largest palindrome made from the product of two 2-digit numbers is 9009 = 91 × 99.

Find the largest palindrome made from the product of two 3-digit numbers.
"""
def is_palindrome(N):
    N_str = str(N)
    chars = []
    for char in N_str:
        chars.append(char)
    ret = True
    if len(N_str) % 2 == 0:
        for i in range(len(N_str)/2):
            if chars[i] == chars[len(N_str)-i-1]:
                pass
            else:
                ret = False
                return False
    else:
    #if len(N_str) % 2 == 1
    for i in range(math.ceil(len(N_str)/2.0)):
        if chars[i] == chars[len(N_str)-i-1]:
            pass
        else:
            ret = False
            return False
    if ret = True:
        return True
        
palindromes = []
for i in range (999, 99, -1):
    for j in range(999, 99, -1):
        product = ij
        if is_palindrome(product):
            palindromes.append(product)
            
answer = max(palindromes)
print(answer)
