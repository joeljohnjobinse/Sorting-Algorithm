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
Developed by: Joel John Jobinse
RegisterNumber: 212223240062
'''
def selection_sort(array,size):
    for ind in range(size):
        min_index=ind
        for j in range(ind+1,size):
            if array[j]<array[min_index]:
                min_index=j
        (array[ind],array[min_index])=(array[min_index],array[ind])
list_of_nums = eval(input())
size=len(list_of_nums)
selection_sort(list_of_nums,size)
print(list_of_nums)

```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Joel John Jobinse
RegisterNumber: 212223240062
'''
def insertion_sort(arr):
    n=len(arr)
    if n<=1:
        return
    for i in range(1,n):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=key
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)

```

## Output:
![py4-1](https://github.com/joeljohnjobinse/Sorting-Algorithm/assets/138955488/c273ec2a-6238-466d-a2b8-2579c66f2f02)
![py4-2](https://github.com/joeljohnjobinse/Sorting-Algorithm/assets/138955488/06857d22-bf9e-4390-9050-073ef7c1ffc8)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
