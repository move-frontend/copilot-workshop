# Effective Prompting for GitHub Copilot

This guide provides proven prompting techniques to help you get the most out of GitHub Copilot. The way you communicate with Copilot significantly impacts the quality and relevance of its suggestions.

## Core Principles of Effective Prompting

1. **Be Specific**: Include details about what you want
2. **Provide Context**: Help Copilot understand your project and goals
3. **Use Examples**: Show patterns you want Copilot to follow
4. **Iterate**: Refine your prompts based on responses
5. **Break Down Complex Tasks**: Split complicated problems into smaller parts

## Code Completion Prompts

### Function Implementation

#### ✅ Effective:

```javascript
// Implement a debounce function that limits how often a function can be called
// It should take a function, delay time in ms, and an option for leading/trailing execution
// Similar to lodash debounce but simplified
```

#### ❌ Less Effective:

```javascript
// Create debounce
```

### Data Transformation

#### ✅ Effective:

```javascript
// Parse CSV string into array of objects, handle quoted fields with commas
// Input format: "name,age,city" with header row
// Return array of objects like {name: "John", age: 30, city: "New York"}
```

#### ❌ Less Effective:

```javascript
// CSV parser
```

### Error Handling

#### ✅ Effective:

```javascript
// Implement try/catch for the API call below with specific error handling:
// - Log and retry once on network errors
// - Show user-friendly message on 404
// - Report to monitoring service on 500+ errors
fetch('/api/users');
```

#### ❌ Less Effective:

```javascript
// Add error handling
fetch('/api/users');
```

### Component Creation

#### ✅ Effective:

```jsx
// Create a React component for a responsive image gallery
// - Accept an array of image objects (url, alt, title)
// - Show thumbnails that open full-size on click
// - Include left/right navigation and keyboard controls
// - Lazy load images for performance
```

#### ❌ Less Effective:

```jsx
// Make an image gallery
```

## Function Signature Approach

Defining function signatures is a powerful way to guide Copilot:

```javascript
/**
 * Filters and sorts a product list based on multiple criteria
 * @param {Object[]} products - Array of product objects
 * @param {Object} filters - Filter criteria (category, price range, rating)
 * @param {string} sortBy - Sort field (name, price, rating)
 * @param {boolean} ascending - Sort direction
 * @returns {Object[]} Filtered and sorted product array
 */
function filterAndSortProducts(products, filters, sortBy, ascending) {
  // Let Copilot implement the function body
}
```

## Copilot Chat Prompts

### Code Explanation

#### ✅ Effective:

```
Can you explain how this authentication middleware works? I'm especially
confused about how the JWT verification interacts with the user lookup process.

[paste code here]
```

#### ❌ Less Effective:

```
Explain this code

[paste code here]
```

### Debugging Help

#### ✅ Effective:

```
I'm getting this TypeError: "Cannot read property 'filter' of undefined" in my React component.
Here's the component code and the data structure I'm working with. Can you help identify what's causing this and suggest a fix?

[paste code and data structure]
```

#### ❌ Less Effective:

```
My code has an error, please fix it.

[paste code]
```

### Learning Concepts

#### ✅ Effective:

```
Can you explain React's useEffect hook? Specifically:
1. How it compares to class component lifecycle methods
2. Common patterns for data fetching
3. How to properly handle cleanup
4. Best practices for dependency arrays

Include simple examples for each point.
```

#### ❌ Less Effective:

```
Tell me about useEffect
```

### Architecture Guidance

#### ✅ Effective:

```
I'm building a Node.js API that needs to process large CSV file uploads (100MB+),
parse them, validate the data, and import it into a MongoDB database. The process
should be resumable if interrupted. What architecture would you recommend?
Consider performance, error handling, and monitoring.
```

#### ❌ Less Effective:

```
How to build an API for file uploads?
```

## Multi-File Implementation

When implementing features across multiple files, provide context about the overall structure:

```
I have a React application with the following structure:
- src/components/UserProfile.jsx (displays user info)
- src/api/userService.js (handles API calls)
- src/store/userSlice.js (Redux state)

I need to add a "change password" feature that:
1. Adds a form to UserProfile.jsx
2. Creates an API method in userService.js
3. Updates the Redux state in userSlice.js

Help me implement the necessary changes in each file.
```

## Agent Mode Prompts

Agent Mode excels with multi-step problems. Frame your prompt as a collaborative conversation:

```
I'm working on implementing a feature that allows users to export their data in different formats.
I need to:
1. Create a UI component for format selection
2. Implement the export logic for CSV, JSON, and PDF
3. Handle large datasets with pagination
4. Add progress indication for the user

Let's start by planning the approach, then we can implement each part step by step.
```

## Language-Specific Prompts

### Angular

```
Create an Angular service that handles authentication using JWT.
Include methods for login, logout, token refresh, and checking authentication status.
Store tokens in localStorage and add an HTTP interceptor for adding the token to requests.
```

### PHP

```
Implement a PHP class for a shopping cart that:
- Uses sessions to maintain state
- Has methods to add, remove, update quantities
- Calculates totals, tax, and shipping
- Interfaces with a Product class (assume it exists)
- Handles serialization for database storage
```

### Android/Kotlin

```
Create a Kotlin data class for a User model with:
- Basic properties (id, name, email)
- Proper nullability annotations
- Companion object with factory methods
- Extension function for formatted display
- Parcelable implementation for Android
```

## Iterative Prompting

If you don't get the desired result, iterate on your prompt:

### First Attempt:

```
Create a date formatter utility
```

### Refined Attempt:

```
Create a date formatter utility in JavaScript with these features:
- Format dates in different locales (US, EU, custom)
- Convert between timezones
- Calculate relative time (e.g., "2 days ago")
- Handle invalid dates gracefully
- Include unit tests for each function
```

## Troubleshooting Prompts

When Copilot isn't giving you what you need:

1. **Add more details**: Specify language, framework, patterns
2. **Include examples**: Show input/output examples
3. **Use constraints**: Mention performance requirements, coding standards
4. **Break it down**: Ask for one specific part at a time
5. **Provide context**: Explain the problem you're trying to solve

## Project-Specific Prompting

For large projects, help Copilot understand the codebase:

```
In our e-commerce project:
- We use Repository pattern for data access
- Services handle business logic
- DTOs transfer data between layers
- We follow REST API conventions

I need to add a new feature for wishlists. Help me design the necessary
components following our architecture patterns.
```

## Remember

- The quality of Copilot's responses directly correlates to the quality of your prompts
- Copilot may need more context than you think - be generous with details
- You can always refine and iterate on your prompts
- Combine Copilot's suggestions with your own expertise for best results
