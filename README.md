# Step_1
def is_prime(n):   
  d = 2          
  while d * d <= n:
    if n % d == 0:
      return False  
    d += 1
  return True

k = 0
for i in range(1000, 1000001):
  if i % 100 == 21 and is_prime(i):
    k += 1
            
print(k)
