# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1 // Caleb

Arrays, Linked Lists and Doubly Linked Lists all allow programmers to organize data in a sequence. So, how would you choose to use one over the other?

In your response, make sure to compare the time complexities for insertion, removal, and random access (grabbing a particular known element by index/position) for each data structure as well as memory usage and ease of traversal.

### Response 1
You would use an array when you need easy access to your data. Arrays are very easy to traverse through. Arrays generally use less memory per element as they do not require strong pointers. Arrays have a time complexity of O(n) when it comes to insertion and deletion as the array needs to shift elements when it does so. But when it comes to access and retrieval, it only has a time complexity of O(1).

You would use a linked list when you want efficient insertion and deletion of elements. Linked lists have a higher memeory use per element than arrays due to storing data and pointers. Access and retrieval of elements have a time complexity of O(n) as traversing requires starting from the head. Meanwhile, insertion and deletion of an node in a linked list have a time complexity of O(1) when the previous node is known.

You would use a doubly linked list when you need to go back to previous nodes in a linked list efficiently. Other than that, doubly linked lists have the same functionality and use as a regular linked list. Doubly linked lists have the same time complexity as a linked list when it comes to insertion and deletion, as well as when it comes to access and retrieval.



## Prompt 2 // Caleb

Imagine you are developing a web browser's "back" button functionality. When a user clicks "back," the browser should navigate to the previously visited webpage. 

Would you use a stack or a queue to implement this functionality? 

In your response, explain what a Stack/Queue is and why it would be best for this use case. Make sure that your response includes the terms LIFO or FIFO.

### Response 2
 For the functionality of the browser's "back" button, I would use a stack to implement the functionality.
 Due to the Last In, First Out principle that the data structure is based on, it would be easy to bring back the functionality of going back to a previously visited webpage.

 A queue would not be good to use to implement this functionality due to its First In, First Out principle that the data structure is based off of. If you were to implement this functionality with queues, it would be slow since the back button would have to go to the back of the queue and wait for everything else to finish.

## Prompt 3

What is an Abstract Data Type and why are they worth learning about?

### Response 3

## Prompt 4

A few classic problems involving a stack are the `isBalanced` and `isPalindrome` functions. Choose one of these functions and provide a solution to it along with a brief lesson explaining how it works. 

### Response 4



