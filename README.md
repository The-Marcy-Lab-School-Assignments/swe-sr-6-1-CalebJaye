# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Arrays, Linked Lists and Doubly Linked Lists all allow programmers to organize data in a sequence. So, how would you choose to use one over the other?

In your response, make sure to compare the time complexities for insertion, removal, and random access (grabbing a particular known element by index/position) for each data structure as well as memory usage and ease of traversal.

### Response 1

## Prompt 2

Imagine you are developing a web browser's "back" button functionality. When a user clicks "back," the browser should navigate to the previously visited webpage.

Would you use a stack or a queue to implement this functionality?

In your response, explain what a Stack/Queue is and why it would be best for this use case. Make sure that your response includes the terms LIFO or FIFO.

### Response 2

## Prompt 3

What is an Abstract Data Type and why are they worth learning about?

### Response 3

An Abstract Data Type (ADT) is a data type defined from the user’s perspective rather than its underlying implementation. Common ADTs include lists, stacks, queues, deques, and more. ADTs are worth learning because they can benefit your code in many ways. They can optimize both space and time complexity. For example, using a hash table can make data retrieval faster. Since they are defined from the user’s perspective, ADTs are more likely to be reusable across different scenarios during implementation and coding.

## Prompt 4

A few classic problems involving a stack are the `isBalanced` and `isPalindrome` functions. Choose one of these functions and provide a solution to it along with a brief lesson explaining how it works.

### Response 4

The **isPalindrome** problem is a well-known coding challenge that can be solved using a **stack**.

## **What is a Stack?**

A **stack** is a data structure that follows the **LIFO (Last In, First Out)** principle. This means that the **last item added** to the stack is the **first one removed**.

## **Stack Implementation in JavaScript**

```javascript
class Stack {
  constructor() {
    this.items = [];
  }

  push(element) {
    this.items.push(element);
  }

  pop() {
    return this.items.pop();
  }

  isEmpty() {
    return this.items.length === 0;
  }
}

const isPalindrome = (inputString) => {
  let stack = new Stack();

  for (let char of inputString) {
    stack.push(char);
  }

  for (let char of inputString) {
    if (char !== stack.pop()) {
      return false;
    }
  }

  return true;
};
```

## **How It Works**

1. **Create a Stack**
   - We start by **creating a new stack** using the previously defined `Stack` class.
2. **Push Characters into the Stack**
   - We iterate over the input string using a `for...of` loop and **push each character** onto the stack.
3. **Compare Characters While Popping**
   - We **pop** characters from the stack **one by one** and compare them to the original string.
4. **Return Result**
   - If a mismatch is found, return `false` (not a palindrome).
   - If all characters match, return `true` (it is a palindrome).
