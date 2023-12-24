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
Developed by: Naveenkanthan L
RegisterNumber: 23007705
'''
def selection_sort(array):
    length=len(array)
    for i in range(length-1):
        minIndex=i
        for j in range(i+1,length):
            if array[j]<array[minIndex]:
                minIndex=j
        array[i],array[minIndex]=array[minIndex],array[i]
    return array
    
array=eval(input())
print(selection_sort(array))
```
ii)	#Insertion Sort
```
def insertion_sort(array):
    n=len(array)
    if n<=1:
        return
    for i in range(1,n):
        key=array[i]
        j=i-1
        while j>=0 and key<array[j]:
            array[j+1]=array[j]
            j-=1
        array[j+1]=key
        
array=eval(input())
insertion_sort(array)
print(array)
```

## Output:
### selection
<img width="576" alt="290184859-dd130a4b-4b0c-45eb-9e44-d4af00f97c60" src="https://github.com/Naveen1825/Sorting-Algorithm/assets/138969868/26fb3347-3b86-42e8-b77f-5bb4aa33a6b8"><br>
### isertion
<img width="574" alt="290185007-5f9143df-54f8-44a2-be97-5cc3c605390b" src="https://github.com/Naveen1825/Sorting-Algorithm/assets/138969868/1c91eb3f-521a-4e30-8e36-269223315d49"><br>
## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
