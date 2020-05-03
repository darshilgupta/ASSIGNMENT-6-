# ASSIGNMENT-6-
Bottle neck
def min_visible_bottles(arr, n): 
  
    m = dict() 
    ans = 0
    for i in range(n): 
        m[arr[i]] = m.get(arr[i], 0) + 1
        ans = max(ans, m[arr[i]]) 
  
    print("Minimum number of", "Visible Bottles are: ", ans) 
  

n = int(input())
arr = list(map(int,input().split(" ")))
min_visible_bottles(arr, n)
