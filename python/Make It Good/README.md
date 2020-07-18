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

---
## Question Analysis


Python WriteUps/Code:
- [ ] [Count Divisors](https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/count-divisors/) -- Kingold 
- [ ] [e-maze-in](https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/e-maze-in-1aa4e2ac/) -- Rose
- [ ] [IT’S MAGIC!](https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/its-magic/) -- Evangeline
- [ ] [Two Strings](https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/two-strings-4/) -- Jia Xiang
- [ ] [Friend's Relationship](https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/friends-relationship-1/) -- Hongshuo
- [ ] [Ali and Helping innocent people](https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/cartag-948c2b02/) -- Joel
- [ ] [Make It Good](https://codeforces.com/contest/1385/problem/C) -- Isaac

---

The write-up (**if its a md file**) should be in the format below:

# _insert question name here_

**Question link:** _insert question url here_

**Question description:**

_insert the question description here. copy pasting from the site itself would work_

**Question solution:**

_insert your solution here. you can add pictures, gifs, videos etc... but most importantly is your thought process when solving this question. Do note: if you wish to include pictures, videos, etc you would need to upload the pictures into the `resources` folder then reference it in your markdown file_

**If it is a python file, do also use the format above, but place it in the comments at the top of the file**

Thanks! :pray:
