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

An example of an application that requires alghoritmitic content is in the field of cryptography. Take for example a cryptographic hash functions that is used to verify the integrity of messages and files. A file that have been tampered with during transfer can be detected by checking if the result of tha algorithm that calculates the hash digest over the message is different than the known expected value.
