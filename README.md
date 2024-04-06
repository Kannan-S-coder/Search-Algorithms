# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```python
#Developed By: Kannan.S
#Register No: 212223230098

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```

ii)	# Find the element in a list using Binary Search(Iterative Method).
```python
#Developed By: Kannan.S
#Register No: 212223230098

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```

iii)	# Find the element in a list using Binary Search (recursive Method).
```python
#Developed By: Kannan.S
#Register No: 212223230098

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```

## Sample Input and Output:
i) #Use a linear search method to match the item in a list.

![unit 3 exp 7(i)](https://github.com/Kannan-S-coder/Search-Algorithms/assets/147120710/cf45c28f-6981-4fbc-9766-aeeadf1d9942)

ii) #Find the element in a list using Binary Search(Iterative Method).

![unit 3 exp 7(ii)](https://github.com/Kannan-S-coder/Search-Algorithms/assets/147120710/1247e4b9-430d-42b7-90ad-791c9ec34710)

iii) # Find the element in a list using Binary Search (recursive Method).

![unit 3 exp 7(iii)](https://github.com/Kannan-S-coder/Search-Algorithms/assets/147120710/7f669ddc-f8a8-480d-ac8e-53544703a750)


## Result
Thus the linear search and binary search algorithm is implemented using python programming.
