# Multi-File Editing Exercise

## Overview

GitHub Copilot's multi-file editing capabilities allow you to make coordinated changes across several files in your project. This exercise will teach you how to leverage Copilot's understanding of your project structure to implement features that span multiple components.

## Learning Objectives

- Use Copilot to understand relationships between files in your project
- Generate consistent implementations across multiple files
- Coordinate changes that need to happen in several locations
- Refactor code that spans multiple components

## Prerequisites

- GitHub Copilot enabled in your IDE
- A multi-file project to work with (or the employee directory sample project)
- Basic understanding of your project's structure

## Exercise Steps

### Step 1: Understanding Project Structure

1. Open several related files in your project to provide context to Copilot:

   - For a React project: component file, stylesheet, test file
   - For a backend project: controller, model, and route files
   - For any project: Try to open files that would need to be modified together

2. In Copilot Chat, ask for an analysis of the relationships between these files:

   ```
   Can you explain how these open files are related and how they work together?
   ```

3. Review Copilot's explanation of the file relationships

### Step 2: Implementing a Feature Across Files

1. Identify a feature that would require changes in multiple files. For example:

   - Adding a new data field that needs to be displayed, validated, and stored
   - Creating a new API endpoint with corresponding frontend components
   - Implementing a new theme option throughout the UI

2. In Copilot Chat, describe the feature you want to implement:

   ```
   I want to add a "darkMode" theme option to our application. It should be toggleable in the header, stored in user preferences, and affect the UI styling. What files would need to be modified?
   ```

3. Review Copilot's suggestions about which files need to be changed

4. Ask for specific implementation details for one file:

   ```
   Show me how to implement the dark mode toggle in the Header component.
   ```

5. Implement the suggested changes in that file

6. Continue asking for implementation details for each required file, maintaining context about the feature

### Step 3: Using Copilot to Navigate Between Files

1. In Copilot Chat, ask about where a specific functionality is implemented:

   ```
   Where in our codebase is the user authentication logic implemented?
   ```

2. If Copilot identifies files that aren't currently open, open those files

3. Ask Copilot to explain how those files work together:

   ```
   How does the authentication flow work across these files?
   ```

4. Use this understanding to make coordinated changes across the files

### Step 4: Refactoring Across Files

1. Identify a piece of functionality that's implemented across multiple files but could be improved

2. Share your refactoring idea with Copilot Chat:

   ```
   I want to refactor our form validation to use a centralized validation library instead of having validation logic in each component. How should I approach this?
   ```

3. Ask for specific steps to implement this refactoring:

   ```
   What should the new validation utility file look like?
   ```

   ```
   How would I modify the UserForm component to use this new validation utility?
   ```

4. Implement the changes as suggested, making sure to maintain consistency across files

## Challenge Activities

Now try these challenges to practice multi-file editing:

### Challenge 1: Add a New Feature

Create a new feature that requires changes in at least three different files. For example:

- Add a user notification system (UI component, state management, API integration)
- Implement a data export feature (UI button, API endpoint, file generation)
- Create a new form with validation and state management

Use Copilot to help you identify the necessary files and implement the changes consistently.

### Challenge 2: Cross-Component Refactoring

Identify a pattern that's repeated across multiple components and refactor it into a shared utility or component. For example:

- Extract common form field validation into a shared utility
- Create a reusable UI component from repeated patterns
- Centralize API calling patterns into a service

Ask Copilot to help you with both the extraction and the updates to all affected files.

### Challenge 3: Implement a Design Pattern

Choose a design pattern (like Observer, Factory, Repository, etc.) that would benefit your project and implement it across multiple files. Use Copilot to:

1. Design the pattern implementation
2. Create the necessary files
3. Modify existing code to use the new pattern
4. Ensure consistency across the implementation

## Tips for Success

- Open relevant files before asking Copilot about multi-file changes
- Be specific about the feature or change you want to implement
- Break down complex multi-file changes into manageable steps
- Use Copilot Chat to understand file relationships before making changes
- Check for consistency across implementations in different files
- Remember that Copilot has limited context outside of open files
- Use Copilot's suggestions as a starting point and adapt them to your specific project structure

## Next Steps

Once you've completed this exercise:

- Explore the [GitHub Web Integration Exercise](./github-web-exercise.md) to learn how to use Copilot on GitHub.com
- Apply multi-file editing techniques to your own projects
- Try combining multi-file editing with Agent Mode for complex feature implementations
