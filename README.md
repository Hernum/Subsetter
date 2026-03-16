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
1:Get the largest number from the list that is under (x minus the smallest number in the list).
2:Calculate the remain of the first iteration.
3:Get the second largest number under x.
4:Get the remain of the next iteration.
5:Once the remain is <0, you know you have hit the floor(or x), if all values are used before this happens, return 1;
6:Choose iterativly smaller numbers until the remain is above 0 again(You replace the number that overshot).
7:If none succeeded, remove the biggest scope wich does not make (remain > sum_of_left_over_num)
8:

// Gonna dissapear for a week again but i will finish this. I am onto somthing.
