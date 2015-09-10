# PROJET-EULER
Projet EULER

#PROBLEM 1

import time
 
start = time.time()
 
s = sum([i for i in range(1000) if (i % 3 == 0 or i % 5 == 0)])
 
elapsed = time.time() - start
 
print "result %s returned in %s seconds" % (s,elapsed)

#PROBLEM 2

prev, cur = 0, 1

total = 0

while True:

prev, cur = cur, prev + cur

    if cur >= 4000000:
        break
    if cur % 2 == 0:
        total += cur
print(total)

#PROBLEM 3

def Euler3(n=600851475143):
    for i in range(2,100000):
        while n % i == 0:
            n //= i
            if n == 1 or n == i:
                return i
