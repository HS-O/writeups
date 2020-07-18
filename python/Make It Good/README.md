# Make It Good

_Question is extremely long, so you can find it here at [this contest link](https://codeforces.com/contest/1385/problem/C)_

tl;dr: This question involves an array 𐤀 of size n. 𐤀 needs to be made into a _good_ array, where a _good_ array is defined by an array which can be completely made into a non-decreasing array by transferring either the first or last element one by one. Here's an example:

b = [1,2,3,4,4,2,1] . This array is _good_ because we can obtain a non-decreasing array c from it by the following sequence of operations:

take the first element of b, so b=[2,3,4,4,2,1], c=[1]<br/>
take the last element of b, so b=[2,3,4,4,2], c=[1,1]<br/>
take the last element of b, so b=[2,3,4,4], c=[1,1,2]<br/>
take the first element of b, so b=[3,4,4], c=[1,1,2,2]<br/>
take the first element of b, so b=[4,4], c=[1,1,2,2,3]<br/>
take the last element of b, so b=[4], c=[1,1,2,2,3,4]<br/>
take the only element of b, so b=[], c=[1,1,2,2,3,4,4] — c is non-decreasing.

To make 𐤀 into a _good_ array, we can remove a prefix of size 𐡀, where a prefix is defined as a subarray starting from the first element of 𐤀. The task is to find the smallest possible value of 𐡀.

## Question Analysis

This question was given in Codeforces Round #656, and I only made it past 3 questions before deciding to sleep. I did find my solution to the 3rd question quite cool, but I'm not really sure if its the most cost-efficient one.

#### Initial Thoughts

Looking at the question at a glance, you can instantly know what this question is actually asking: Find the longest _good_ array ending at the last element of 𐤀. After you've found the length of this array, simply output the index of the beginning element of the _good_ array, which will be the length of the prefix to remove. Here's an example:

b = [4,3,3,8,4,5,2]. This array is not good yet, but we can see that the longest _good_ array ending at the last element 2 is [4,5,2], which gives a resulting non-decreasing array of [2,4,5]. Since the _good_ array starts at element 4 which is at index 4, the length of the prefix we have to remove is 4 (because an array starts from 0).

