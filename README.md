# CIT281 Project 6

## Overview

Project goals and outcomes:

1. Gain experience creating and working classes with inheritance.
2. Gain more experience creating and working with classes.
3. Gain more experience debugging code.
4. Gain more experience using a generic block of code to process data.
5. Gain more experience interpreting functional descriptions and specifications to complete an assignment.
6. Gain more experience writing and executing non-web server Node.js JavaScript code using VSCode.
7. Practice using modern JavaScript syntax.
8. Gain more experience working with static data.

## Deliverables

- `lab-06.zip`
- `lab-07.zip`
- `p6.js`

These files should be placed in your `cit281/p6` folder and zipped into `p6.zip`.

## Summary

In Project 6, the focus was on creating three classes to understand and implement the concepts of inheritance and class-based design. The `Shape` class served as a base class for the `Rectangle` and `Triangle` classes, demonstrating the principles of inheritance. Key concepts include class construction, method implementation, debugging, and processing static data using modern JavaScript syntax.

### Project Structure
1. **`Shape` Class**:
   - Base class for the `Rectangle` and `Triangle` classes.
   - Constructor that takes an array of sides.
   - Method `perimeter` that calculates the perimeter of the shape using the `reduce` method and ternary operator for an empty array.

2. **`Rectangle` Class**:
   - Inherits from the `Shape` class.
   - Constructor that takes length and width and calls the `Shape` constructor.
   - Method `area` that calculates the area of the rectangle.

3. **`Triangle` Class**:
   - Inherits from the `Shape` class.
   - Constructor that takes three sides and calls the `Shape` constructor.
   - Method `area` that calculates the area of the triangle using Heron's formula.

### Testing and Execution
- Each class was tested individually to ensure correct functionality.
- A generic block of code was created to process an array of side arrays and output the results using various coding techniques such as `for..of`, `switch`, spread operator, template literals, and `toString` method.

### Sample Code Snippets
#### Shape Class Testing
```javascript
console.log(new Shape([5, 10]).perimeter());  // 15
console.log(new Shape([1, 2, 3, 4, 5]).perimeter()); // 15
console.log(new Shape().perimeter()); // 0
