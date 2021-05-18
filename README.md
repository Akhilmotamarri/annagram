# annagram
l=[] #stroring string
d={} #grouping anagrams
for i in range(int(input())):
    a=input()
    l.append(a)
for j in l:
    m=''.join(sorted(j))
    if m not in d:
        d[m]=[]
        d[m].append(j)
    else:
        d[m].append(j)
        
for i in d:
    if len(d[i])>=2:
        print(d[i],"are annagrams")
    else:
        print(d[i],"is not a annagram")
