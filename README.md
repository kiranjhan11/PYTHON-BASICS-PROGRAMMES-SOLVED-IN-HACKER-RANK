# PYTHON-BASICS-PROGRAMMES-SOLVED-IN-HACKER-RANK
N=int(input())
s=[]
b=[]
ki=[]
if N>=2 and N<=5:
    for i in range(N):
        names=input()
        scores=float(input())
        s.append([names,scores])
        b.append(scores)
x=min(b)
for i in range(b.count(x)):
    y=b.index(x)
    s.pop(y)
    b.pop(y)
z=min(b)
for i in range(b.count(z)):
    r=b.index(z)
    ki.append(s[r][0])
    s.pop(r)
ki.sort()
for i in range(len(ki)):
    print(ki[i])
