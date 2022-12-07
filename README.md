# binary-search
def search(lst,low,high,x):
    low=0
    high=n-1
    while low<=high:
        mid=int(low+(high-low)/2)
        if(lst[mid]==x):
            return mid
        elif(lst[mid]<x):
            low=mid+1
        else:
            high=mid-1
lst=[]
n=int(input())
for i in range(0,n):
    elem=int(input())
    lst.append(elem)
x=int(input("enter elem to search"))
res=search(lst,0,n-1,x)
if(res==-1):
    print("not found")
else:
    print("elem is at index",res)

