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
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: AJITH KUMAR A
RegisterNumber: 23002150

'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i] 
    print(nums)    
list_of_nums = eval(input())
selection_sort(list_of_nums)
# use the selection sort function
# print the sorted list







```
ii)	#Insertion Sort
```

''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: AJITH KUMAR A
RegisterNumber: 23002150
'''
def insertion_sort(nums):
    for i in range(len(nums)):
        insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>insert:
          nums[j+1]=nums[j]
          j-=1
        nums[j+1]=insert
    print(nums)    
list_of_nums = eval(input())
insertion_sort(list_of_nums)




```

## Output:
![image](https://github.com/Ajith1413/Sorting-Algorithm/assets/139842524/ae000fe6-ce58-444b-b833-5e5069f3d63e)
![image](https://github.com/Ajith1413/Sorting-Algorithm/assets/139842524/2d9a7173-42b7-4de3-a898-95a39008a262)
![image](https://github.com/Ajith1413/Sorting-Algorithm/assets/139842524/af326265-1aa2-47e7-8f27-4762317739c8)
![image](https://github.com/Ajith1413/Sorting-Algorithm/assets/139842524/9f1f36b4-17fe-4653-92c6-15efaab7ae6f)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
