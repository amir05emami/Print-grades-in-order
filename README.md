# Print-grades-in-order
l1 = []
l2 = []
while 1:
    n = input("name: ")
    if n =="":
        break
    s = float(input("score: "))
    l1.append(n)
    l2.append(s)
d = len(l2)    
for i in range(1,d+1):
    if len(l2)!=0:
        x= l2.index(max(l2))
        print(f"{i}. name = {l1[x]}     score = {l2[x]}")
        l2.pop(x)
        l1.pop(x)
    else:
        break 
