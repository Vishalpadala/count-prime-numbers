# count-prime-numbers
class Solution(object):    
   def countPrimes(self, n):      
 count = 0       
primes = [False for i in range(n+1)]       
for i in range(2,n):         
 if primes[i] == False:            
 count+=1            
 j = 2            
 while j*i&lt;n:               
 primes[j * i] = True              
  j+=1      
 return count 
ob1 = Solution()
 n=int(input(".   ")) 
print(ob1.countPrimes(n))
