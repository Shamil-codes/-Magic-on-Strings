# -Magic-on-Strings
def prefsum(inputlist):
    outlist = []
    for i in range(1, len(inputlist)+1):
        nextvalue = sum(inputlist[:i])
        outlist.append(nextvalue)
    return outlist
K = 10
Q = 5
list0 = [1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1]
for i in range(Q):
    nextlist = prefsum(list0)
    list0 = nextlist[:]
print(nextlist[K]%1000000007)
