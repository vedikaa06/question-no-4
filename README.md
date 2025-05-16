# question-no-4
Solution to the question no 4 on leet code 

4. Median of Two Sorted Arrays

Given two sorted arrays nums1 and nums2 of size m and n respectively, return the median of the two sorted arrays.

The overall run time complexity should be O(log (m+n)).

Soultion:

How it works:
Two pointers p1 and p2 track positions in nums1 and nums2.

getMin() returns the smaller of the two current elements and moves the corresponding pointer forward.

The method simulates merging the two arrays until it reaches the middle:

If the total length is even, it takes the average of the two middle values.

If it's odd, it returns the middle value.

Key idea:
Instead of merging the full arrays, it only goes up to the middle to save time.
