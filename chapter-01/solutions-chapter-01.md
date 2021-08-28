# Exercise Solutions Chapter 1

## 1.1-1

A real world example that requires sorting is how to organize merchandise in a store by appropriate grouping. For example dairy in one section, fruit and vegetables in another, frozen foods in the freezer and so on. This prevents food from going bad, and makes it easier for the customer to find products, which greatly increases profit.

A real world example that requires computing a convex hull is packaging of items in boxes. After having calculated the three-dimensional convex hull it is possible to choose the smallest possible box, minimizing the costs of boxes, shipping, and storage.

## 1.1-2

Other than speed so might one measure efficiency by taking memory consumption and network traffic load into account.

## 1.1-3

A data structure that you might have seen previously is the the singly linked list, below is a discussion about its strengths and limitations.

Strengths:

- Insertion of a new element is a fast constant time operation

- Deletion of an existing element is a fast constant time operation

- Number of elements can be changed dynamically at run time

Weaknesses:

- The pointer to the next element in the linked list takes up memory

- Random access is slow compared to storing the data in an array

- No guarantee that the elements are located close in memory which can have a negative effect on caching performance

## 1.1-4

The shortest-path and traveling-salesman problems are similar due to that the goal of both problems is to minimize the length of a path. They are different due to that only two stops are required in the first problem and a stop will only be visited once, in the second problem so are all stops required and a stop might be passed by more than one time.

## 1.1-5

A real world problem in which only the best solution will do is sorting words into a dictionary. A word not placed in the correct alphabetical order will make it time consuming to find the word and its explanation.

A real world problem in which a solution that is "approximately" the best is good enough is weather forecasts. A forecast is always just approximately right but still adds value to the user that want to choose what clothes to pack when for example traveling away over a weekend.

## 1.2-1

An example of an application that requires alghoritmitic content is cryptography. Take for example a cryptographic hash functions that is used to verify the integrity of messages and files. To check that a file have not been tampered with during transfer so can the hash algorithm be applied with the file as input to produce the hash digest and then check that this result is the expected.

## 1.2-2

Lets compare implementations of insertion sort and merge sort on the same machine. For inputs of size n, insertion runs in 8n&#x00B2; steps, while merge sort runs in 64n lg n steps. The goal is to check for which values of n that insertion sort beat merge sort.

Start with the minimal value n = 2. Then for insertion sort we get 32 and for merge sort we get about 38. So insertion sort is better for small values.

To find the n where merge sort starts to outperform insertion sort we need to solve the equation:

8n&#x00B2; < 64n lg n

Divide both sides by 8n to get:

n < 8 lg n

Divide by 8 to get:

n / 8 < lg n

It now turns out that elementary math will not be enough to solve the equation. Since we got stuck lets change strategy and instead start testing different values.

To get an initial estimate fast we try with doubling n every time and then we get:

n = 4 &#x21D2; 4 / 8 < lg 4 &#x21D2; 0.5 < 2

n = 8 &#x21D2; 8 / 8 < lg 8 &#x21D2; 1 < 3

n = 16 &#x21D2; 16 / 8 < lg 16 &#x21D2; 2 < 4

n = 32 &#x21D2; 32 / 8 < lg 32 &#x21D2; 4 < 5

n = 64 &#x21D2; 64 / 8 < lg 16 &#x21D2; 8 < 6

We can now deduce that insertion sort wins for n = 32 but is slower for n = 64. To find the exact limit we can use a calculator to test values in between 32 and 64. This is fast enough to brute force on the calculator since maximum 30 values needs to be tested.

Note that you can also speed up the process using a binary search by starting in the middle of the 32 to 64 interval and test 48 first and then proceed from there with the next middle point in a new smaller interval.

After having used the calculator to narrow down the range so will we eventually find that:

n = 43 &#x21D2; 43 / 8 < lg 43 &#x21D2; 5.375 < 5.426

n = 44 &#x21D2; 44 / 8 < lg 43 &#x21D2; 5.500 < 5.459

This means that we have the solution. For n from 2 up to 43 so will insertion sort be faster but when n is 44 and above so will merge sort perform better.
