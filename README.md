Download Link: https://assignmentchef.com/product/solved-csd235-335-assignment-2-quick-sort
<br>
For this programming assignment you will implement Quick Sort and execute it with 4 separate data sets. Each data set is a 1,000,000 element integer array, organized as follows:

random

nearly sorted ascending ( sorted ascending data set with small number of elements out of order) sorted ascending sorted descending

There are a number of different implementations of Quick Sort. Your implementation should start with the pseudo coded Quick Sort algorithm presented in figure 3.5.1 of the zybook used for this course, with the modifications that follow.

Add a call to System.nanoTime() immediately before, and immediately after the call to Quick Sort to calculate how much time elapsed during the sorts. Output these values along with a description of what’s being measured.

<h2>Median-of-Three Partitioning</h2>

The optimal choice for a pivot would be the median of the array. However, this is difficult to calculate and would slow down Quick Sort significantly.  One approach is to pick three elements randomly , and use the median of these three as the pivot. As it turns out, the randomness doesn’t help much. So instead, just use median of the first, last, and center elements as the pivot. For example, if you have the following values for input:

the first value is 17, the last value is 1, and the center value is 13. So in this case the pivot is 13.

Modify your implementation of Quick Sort to choose a pivot using Median-of-Three.

<h2>When the Sub-Arrays Get Small</h2>

Quick Sort is a recursive divide and conquer algorithm. As the recursive descent progresses, sooner or later the sub-arrays will get small enough that Quick Sort doesn’t perform as well as other sortin

algorithms. One possible remedy for this phenomenon is to switch to a sorting algorithms that is efficient for small arrays.

Modify your implementation of Quick Sort to switch to Selection Sort when the length of a sub-array is less than or equal to 20 elements.