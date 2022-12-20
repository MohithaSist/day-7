# day-7

addition of alternate no

a=list(map(int,input().split()))
if ((len(a)==4) and max(a)==a[0] and a[-1]>a[1] and a[-1]>a[2]):
    s1=a[0]+a[-1]
    print(s1)
else:
    d=a[a.index(max(a))::2]
    #print(d)
    e=a[a.index(max(a))::-2]
    #print(e)
    b=e[1::]
    l=d+b
    #print(l)
    s=sum(l)
    print(s)
