import sys
import itertools


#we need to create a graph
#then we need to add edges to each vertex : there needs to be 
#a connection to each var outside of its clause, except for its own negation

#read in boolean 


args = list(sys.argv[1].split())

arr1 = [args[0], args[1], args[2]]
arr2 = [args[3], args[4], args[5]]
arr3 = [args[6], args[7], args[8]]

arr12 = list(itertools.product(arr1, arr2, repeat = 1))
arr13 = list(itertools.product(arr1, arr3, repeat = 1))
arr23 = list(itertools.product(arr2, arr3, repeat = 1))

numedges = len(arr1)*len(arr2)+len(arr1)*len(arr3)+len(arr2)*len(arr3)
#if 
for tuple in arr12:
    if tuple[0][0] != tuple[1][0]:
        if tuple[0][len(tuple[0])-1] == tuple[1][len(tuple[1])-1]:
            numedges -= 1
for tuple in arr13:
    if tuple[0][0] != tuple[1][0]:
        if tuple[0][len(tuple[0])-1] == tuple[1][len(tuple[1])-1]:
            numedges -= 1
for tuple in arr23:
    if tuple[0][0] != tuple[1][0]:
        if tuple[0][len(tuple[0])-1] == tuple[1][len(tuple[1])-1]:
            numedges -= 1            
    
print(numedges)
#print (arr12[0][0])
#print (arr12)
#print (arr13)
#print (arr23)

