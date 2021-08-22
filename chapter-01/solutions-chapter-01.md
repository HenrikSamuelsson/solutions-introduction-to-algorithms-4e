# Chapter 1 Exercise Solutions

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

- Number of elements can be changed up and down dynamically at run time

Weaknesses:

- The pointer to the next element in the linked list takes up memory

- Random access is slow compared to storing the data in an array

- No guarantee that the elements are located close in memory which can have a negative effect on caching performance
