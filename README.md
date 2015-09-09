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
