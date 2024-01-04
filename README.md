# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```python
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by:VASANTHARAJ J
RegisterNumber: 23012935
'''
def selection_sort(nums):

    for i in range(0,len(nums)):
        min_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[min_index]:
                min_index=j
        nums[i],nums[min_index]=nums[min_index],nums[i]
    print(nums)    
   
    
    
    
list_of_nums = eval(input())
selection_sort(list(list_of_nums))
# use the selection sort function
# print the sorted list

```
ii)	#Insertion Sort
```
def insertion_sort(nums):
    # Write your code here to sort the elements in the list using Insertion sort algorithm
    n=len(nums)
    for i in range(1,n):
        key = nums[i]
        j=i-1
        while j>=0 and key <nums[j]:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1] = key
    print(nums)    
    
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)
# use the insertion sort function to get the sorted list
# print the sorted list

```

## Output:
i)	#Selection Sort

![image](https://github.com/Vasanth2k4/Sorting-Algorithm/assets/147139769/164a6530-f515-4d98-a33f-fff16eb073e2)

ii)	#Insertion Sort

![image](https://github.com/Vasanth2k4/Sorting-Algorithm/assets/147139769/7436ab2f-c9fc-479f-bf15-f3a70943cdfc)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
