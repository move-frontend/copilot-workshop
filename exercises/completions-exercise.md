# Code Completions Exercise

## Overview

GitHub Copilot's core functionality provides real-time code suggestions as you type. In this exercise, you'll learn how to effectively use these inline code completions to write code more efficiently while maintaining control over what gets implemented.

## Learning Objectives

- Use GitHub Copilot to generate inline code completions
- Evaluate and refine suggestions for your specific needs
- Apply effective commenting techniques to get better suggestions
- Understand the different ways to navigate between multiple suggestions

## Prerequisites

- GitHub Copilot enabled in your IDE
- Basic familiarity with your chosen programming language
- Basic understanding of the project structure

## Exercise Steps

### Step 1: Basic Code Completion

1. Create a new file in your project directory called `completions_demo.js`

2. Type a descriptive comment about what you want to implement:

   ```javascript
   // Create a function that calculates the factorial of a number
   ```

3. Press **Enter** after typing this comment

4. Observe GitHub Copilot's suggestion for implementing a factorial function

5. Accept the suggestion by pressing **Tab**

6. Review the implemented function to understand Copilot's approach

> 💡 **Tip:** The more specific your comment, the better Copilot's suggestion will be.

### Step 2: Exploring Alternative Suggestions

1. Add another comment for a different function:

   ```javascript
   // Function to check if a string is a palindrome
   ```

2. Press **Enter** after typing this comment

3. If Copilot shows a suggestion but you'd like to see alternatives:

   - Press **Alt+]** (or **Option+]** on Mac) to see the next suggestion
   - Press **Alt+[** (or **Option+[** on Mac) to see the previous suggestion

4. When you find a suggestion you prefer, press **Tab** to accept it

### Step 3: Using Function Signatures to Guide Suggestions

1. Add a new function signature with a comment:

   ```javascript
   /**
    * Sorts an array of objects based on a specified property
    * @param {Array} items - The array of objects to sort
    * @param {string} property - The property to sort by
    * @param {boolean} ascending - Whether to sort in ascending order
    * @returns {Array} The sorted array
    */
   function sortByProperty(items, property, ascending) {
   ```

2. Press **Enter** and see how Copilot completes the function based on the signature and documentation

3. Accept the suggestion by pressing **Tab**

### Step 4: Using Existing Code as Context

1. Add the following incomplete code:

   ```javascript
   const users = [
     { name: 'Alice', age: 32, role: 'developer' },
     { name: 'Bob', age: 45, role: 'manager' },
     { name: 'Charlie', age: 27, role: 'designer' },
   ];

   // Filter users by
   ```

2. After typing the comment, press **Enter** and observe how Copilot uses the existing code as context for its suggestions

3. Try different variations like:

   ```javascript
   // Filter users by role
   ```

   or

   ```javascript
   // Filter users older than 30
   ```

4. Notice how the specificity of your comment influences the generated code

## Challenge Activities

Now that you've learned the basics, try these challenges on your own:

### Challenge 1: Data Transformation

Write a function that transforms an array of numbers by applying a mathematical operation (like squaring or doubling) to each element. Start with:

```javascript
// Function to transform each element in an array by applying a mathematical operation
```

### Challenge 2: API Request Helper

Create a function that makes an API request with error handling and response parsing. Start with:

```javascript
// Function to fetch data from an API with proper error handling
```

### Challenge 3: Complex Data Processing

Implement a function that processes a dataset to generate statistics (min, max, average, etc.). Try to get Copilot to implement this by providing clear comments and function signatures.

## Tips for Success

- Provide detailed, descriptive comments about what you want to implement
- Use JSDoc or similar documentation formats to give Copilot more context
- If you're not happy with a suggestion, try rephrasing your comment or adding more details
- Remember that you can always modify Copilot's suggestions after accepting them
- When working with complex logic, try breaking down the problem into smaller parts
- Use variable and function names that clearly describe their purpose

## Next Steps

Once you've completed this exercise:

- Explore the [Copilot Chat Exercise](./chat-exercise.md) to learn how to interact with Copilot conversationally
- Try applying these techniques to your own projects or the workshop challenges
- Check out the [Effective Prompts](../resources/effective-prompts.md) for more examples of good prompting techniques
