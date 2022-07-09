# Ass-2-9-7-22
Assignemt-2
import math 
n=1000001
seive=[True]*n 
seive[0]=seive[1]=False 
x=int(math.sqrt(n)) 
for i in range(2,x+1):
    for j in range(i*i,n,i):
        seive[j]=False 
N=int(input()) 
count=0 
for i in range(N+1):
    if seive[i]:
        count=count+1 
print(count)
