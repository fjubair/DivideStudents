# Divide Students into Teams

Assume that you are the teacher of a classroom with *n* students. Furthermore, assume that each student *S* is given a score  *C*. Your goal is to divide the students into *m* groups under the following constraint: two students *Si* and *Sj* can be the same group only if the absolute difference between their scores is bound by a distance *d*, i.e., |*Ci - Cj*| <= *d*. Write a program that computes minimal *m*, i.e., the smallest possible number of groups. Note that each group can have as many students as you want as long as the aforementioned constraint is satisfied. Also, different groups may have different number of students. Finally, more than one student may have the same score.

For example, if we have *n=5* students with the scores {1, 2, 3, 4, 5}, and we are given *d=2*, then the minimal number of groups is *m=2*. One optimal division is {1,2,3} and {4, 5}. Another optimal division is {1,2} and {3,4,5}. While more than one optimal answer may exist, the minimum divisions is always 2.

Let us consider another example. Let us say we have *n=8* students with scores {5, 2, 11, 6, 9, 7, 12, 4} ,and we are given *d=2*, then the minimal number of groups is *m=4*. One optimal divison is {2}, {4 5 6}, {7 9}, {11 12}. Other optimal solutions can also be found but there is no solution with less than four groups because the maximum allowed score difference is 2.

Your task is to implement the **numOfGroups** function in Solution.java. The function takes three input arguments: 
*n*: the numebr of students.
*d*: the maximum allowed score difference for students within the same team.
*scores*: an array containing student scores.

The function returns an integer representing the minimal number of groups.

You are also given ten test cases available in StudentTest.java
