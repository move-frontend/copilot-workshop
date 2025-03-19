# Agent Mode Exercise

## Overview

GitHub Copilot Agent Mode is an advanced conversational capability that maintains context throughout a conversation, helping you tackle complex, multi-step development tasks. This exercise will guide you through using Agent Mode for more sophisticated problem-solving.

## Learning Objectives

- Understand how Agent Mode differs from regular Copilot Chat
- Leverage Agent Mode for multi-step problem solving
- Maintain context across a conversation
- Break down complex tasks into manageable steps with Agent assistance

## Prerequisites

- GitHub Copilot with Agent Mode enabled in your IDE
- Access to GitHub Copilot Business features
- Basic understanding of your project and programming concepts

## Exercise Steps

### Step 1: Activating Agent Mode

1. Open Copilot Chat in your IDE using one of these methods:

   - Use the keyboard shortcut: `Ctrl+Alt+I` (Windows/Linux) or `Ctrl+Cmd+I` (Mac)
   - Click the Copilot Chat icon in the sidebar
   - Use the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and search for "GitHub Copilot Chat"

2. Look for the model dropdown menu at the top of the Copilot Chat panel

3. Select the Agent Mode option (available in GitHub Copilot Business tier)

4. Notice that the chat interface now indicates you're in Agent Mode

### Step 2: Multi-Step Problem Solving

1. Start a conversation with Agent Mode by describing a complex task:

   ```
   I need to implement a user authentication system with JWT tokens for a React application. Can you help me plan and implement this?
   ```

2. Observe how Agent Mode breaks down the problem into logical steps

3. Follow up with clarification questions:
   ```
   What dependencies will I need for this implementation?
   ```
4. Notice how Agent Mode remembers the context of your conversation

5. Ask for implementation details for one specific part:

   ```
   Can you show me how to implement the token verification middleware?
   ```

6. Continue the conversation to explore different aspects of the solution

### Step 3: Refactoring with Agent Mode

1. Share a piece of code that could use refactoring:

   ```javascript
   function processUsers(users) {
     let activeUsers = [];
     let inactiveUsers = [];
     let adminUsers = [];
     let regularUsers = [];

     for (let i = 0; i < users.length; i++) {
       if (users[i].status === 'active') {
         activeUsers.push(users[i]);
       } else {
         inactiveUsers.push(users[i]);
       }

       if (users[i].role === 'admin') {
         adminUsers.push(users[i]);
       } else {
         regularUsers.push(users[i]);
       }
     }

     return {
       active: activeUsers,
       inactive: inactiveUsers,
       admins: adminUsers,
       regular: regularUsers,
     };
   }
   ```

2. Ask Agent Mode to help refactor this code:

   ```
   This function seems inefficient and repetitive. Can you help me refactor it to be more concise and efficient?
   ```

3. Review the suggested solution

4. Ask for further improvements:

   ```
   Can we make this even more concise using a functional programming approach?
   ```

5. Notice how Agent Mode builds on the previous solution

### Step 4: Project Planning and Architecture

1. Describe a feature you want to implement:

   ```
   I want to add a feature to our application that allows users to export data in multiple formats (CSV, JSON, PDF). Can you help me plan the architecture for this?
   ```

2. Discuss the proposed architecture with Agent Mode, asking questions like:

   ```
   What design patterns would be appropriate for this feature?
   ```

   ```
   How would you structure the code to make it easy to add new export formats in the future?
   ```

3. Ask for a specific implementation:

   ```
   Can you show me how to implement the CSV export functionality?
   ```

4. Notice how Agent Mode maintains the context of your architectural discussions

## Challenge Activities

Now try these challenges using Agent Mode:

### Challenge 1: Algorithm Optimization

Share an inefficient algorithm with Agent Mode and ask for help optimizing it. Engage in a back-and-forth conversation to understand the optimization techniques and implement them step by step.

### Challenge 2: Feature Planning

Describe a complex feature for your project (like a recommendation system, analytics dashboard, or real-time collaboration tool) and work with Agent Mode to:

1. Define the requirements
2. Plan the architecture
3. Design the data models
4. Outline the implementation approach
5. Identify potential challenges

### Challenge 3: Code Transformation

Take a piece of code written in one programming language or paradigm and ask Agent Mode to help you transform it to another. For example:

- Converting a class-based React component to a functional component with hooks
- Rewriting a synchronous function to use async/await
- Transforming a procedural algorithm to a functional programming approach

## Tips for Success

- Give Agent Mode comprehensive context about your project and requirements
- Break large problems into smaller, focused discussions
- Don't hesitate to ask follow-up questions or request clarification
- Use Agent Mode for exploratory conversations about architecture and design
- Remember that Agent Mode excels at maintaining context across multiple questions
- Be explicit about your goals and constraints to receive more tailored guidance

## Next Steps

Once you've completed this exercise:

- Try using Agent Mode for a real development challenge in your project
- Explore the [Multi-File Editing Exercise](./multi-file-exercise.md) to learn how Copilot can help with changes across multiple files
- Compare your experience with Agent Mode to regular Copilot Chat to understand the differences
