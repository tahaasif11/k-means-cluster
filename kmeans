x=[15,16,16,19,19,20,20,21,22,28,35,40,41,42,43,47,60,61,65]
import random
from statistics import mean
c1=random.choice(x)
c2=random.choice(x)
tmp=True
while tmp:
    
    if c1<c2:
        break;
    else:
        c1=random.choice(x)
        c2=random.choice(x)
print('input:',x)
flag=0
n=1
Ncount1=0
Ocount1=0
Ncount2=0
Ocount2=0

while flag==0:
    g1=[]
    g2=[]
    t1=[]
    t2=[]
    Ocount1=Ncount1
    Ocount2=Ncount2
    for i in x:
        if abs(c1-i)<abs(c2-i):
            g1.append(abs(c1-i))
            t1.append(i)
        else:
            g2.append(abs(c2-i))
            t2.append(i)
    
    print('Iteration#',n)
    print('centroid of x1:',c1)
    print('centroid of x2:',c2)
    print('value x1',t1)
    print('value x2',t2)
    Ncount1=len(g1)
    Ncount2=len(g2)
    if Ncount1==Ocount1 and Ncount2==Ocount2:
        flag=1
        break
    else:
        n+=1
        c1=round(sum(t1) / len(t1))
        c2=round(sum(t2) / len(t2))
