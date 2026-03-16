# Subsetter
If provided a list of lenght N filled with random integers(or floats), and instructed to give the subset of the list 
  that sums to x, what would that subset be?(assuming that the subset can be very big.)



Quick summary of my game plan:
1: Add a chapter in this ReadMe to explain the method used to conclude the subset.
2: Provide small, bite-sized functions that are easy to read and easy to use and develop.
3: Test the program for validity.

Milestones / To-do list.
[]:Make a file to code in.
[]:Write basic bubble sort function (idk yet how it works :( )
[]:Write the function with recursive backtracking.(ik recursion = bad)
[]:
[]:

Quick summary of how the subset is derived:
1:Get the largest number from the list that is under x.
2:Calculate the remain of the first iteration.
3:Get the second largest number under x.
4:Get the remain of the next iteration.
5:Once the remain is <0, you know you have hit the ceiling, if all values are used before this, return 1;
6:Sum all the numers not used yet. 
7:Use the sum of the numbers to determine the scope at wich to iterate the number.
8: This method is stupid and greedy. It is so close to theoratical perfection.
