#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n). The loop runs 'n' amount of times, so if 'n' is large, the loop is proportionately large.


b) O(nlogn). The inner while loop by itself would have a complexity of log(n), and the outer for loop by itself is O(n). So total complexity is O(nlogn)


c) O(n). The loop runs 'n' amount of times. If 10 bunnies are entered, it will run 10 times.

## Exercise II


O(logn) -- Search halves of current amount of floors until found

create a function that takes n amount of floors
if the egg doesnt break at the current top floor,
    return that floor
if it does break at the current top floor,
    find the middle floor, n/2
    if the egg breaks at the middle floor,
        recursively call the function with the bottom-half floors, so floors 1 through n/2
    else if the egg does break at the middle floor,
        recursively call the function with the top-half floors, so floors n/2 to n

    return floor