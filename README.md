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
  Skip repeated numbers during overshooting, so you do not need to calc all that again(For large lists).
7:If none succeeded, remove the biggest scope wich does not make (remain > sum_of_left_over_num)

Logic optimisations:1:Keep variables for tracking the list_counts so you do not have to do look-ups(with summing items again).
                      Example: Total_outside_list , Total_in_list : Whenever you make a change, keep track of it
                      by changing the variables(Total_outside_list+=n;Total_in_list-=1; when you move an item between lists)
                      This way you can do: If (Total_outside_list + Total_in_list - item_to_remove_step_7 < goal ) {item required}
                    2:i forfor... its on the tip of my tongue...

// Gonna dissapear for a week again but i will finish this. I am onto somthing.
