# GitHub Insights Prompts

This document provides ready-to-use prompts for interacting with GitHub Copilot directly on GitHub.com. These prompts are designed to help you gain valuable insights about repositories, code, and pull requests without leaving your browser.

## Overview

GitHub Copilot is integrated directly into the GitHub.com interface, allowing you to:

- Analyze code and repositories
- Generate and improve pull request descriptions
- Create comprehensive code reviews
- Generate documentation
- Understand unfamiliar codebases

## How to Use These Prompts

1. Navigate to a repository, pull request, issue, or file on GitHub.com
2. Look for the GitHub Copilot icon/button in the interface:
   - In PR descriptions: Look for "Generate with Copilot" button
   - In code view: Look for the Copilot icon in the interface
   - In issues: Look for Copilot-related options in the editor toolbar
3. Click the appropriate Copilot button to activate the AI assistant
4. Enter your prompt in the text field that appears
5. Review and use the insights provided

Note: The exact interface elements may vary as GitHub updates its Copilot integration. Look for GitHub Copilot icons or "Generate with AI" options throughout the interface.

## Repository Analysis Prompts

### Code Understanding

```
Explain the architecture of this repository and how the main components interact with each other.
```

```
Summarize what this file does and how it fits into the larger codebase.
```

```
What design patterns are being used in this repository?
```

```
Identify the key classes/functions in this repository and explain their responsibilities.
```

### Code Quality Analysis

```
Review this code for potential performance issues or bottlenecks.
```

```
Identify any security vulnerabilities in this repository, particularly around user authentication.
```

```
What parts of this codebase would benefit most from refactoring?
```

```
Analyze the complexity of this code and suggest simplifications.
```

## Pull Request Enhancement

### Description Generation

```
Generate a comprehensive description for this pull request that explains the changes and their purpose.
```

```
Create a structured PR description that includes background, changes made, testing performed, and potential impacts.
```

### Testing Suggestions

```
Suggest tests that should be added to cover the changes in this pull request.
```

```
What edge cases should be considered when testing these changes?
```

### Impact Analysis

```
What potential impacts might these changes have on other parts of the codebase?
```

```
Are there any performance implications from these changes that should be noted?
```

## Documentation Generation

### Repository Documentation

```
Create a README for this repository that explains its purpose, installation steps, and usage examples.
```

```
Generate a CONTRIBUTING.md file that explains how to contribute to this project.
```

### Code Documentation

```
Generate JSDoc comments for this function that explain parameters, return values, and examples.
```

```
Create documentation for this API endpoint including parameters, response format, and error handling.
```

## Project Management

### Issue Analysis

```
Based on the issues and PRs, what are the main areas of active development in this repository?
```

```
Suggest a roadmap for this project based on existing issues and pull requests.
```

### Dependency Management

```
What dependencies in this project are outdated and should be updated?
```

```
Analyze the dependencies in this project and identify any that might pose security or compatibility risks.
```

```
Are there any unused dependencies that could be removed from this project?
```

## Code Review Assistance

### Review Comments

```
What code standards or conventions are not being followed in this PR?
```

```
Is this implementation consistent with similar features in the codebase?
```

```
Suggest ways to make this code more maintainable and readable.
```

### Best Practices

```
How could this code be improved to follow modern best practices?
```

```
Are there any potential memory leaks or resource management issues in this code?
```

## Test Coverage Analysis

```
What areas of the codebase appear to lack test coverage?
```

```
Generate unit tests for this component that cover the main functionality and edge cases.
```

```
How could we improve the existing test suite for better coverage?
```

## Performance and Optimization

```
Identify any N+1 query issues in this repository's database access code.
```

```
Are there opportunities to implement caching to improve performance in this codebase?
```

```
Suggest ways to optimize the frontend bundle size based on the configuration files.
```

## Issue Templates

```
Create a detailed issue template for bug reports that would be appropriate for this repository.
```

```
Generate a feature request template that captures requirements and acceptance criteria.
```

## Specialized Analysis Prompts

### Dark Mode Implementation Analysis

```
I'd like a comprehensive analysis of dark mode implementation in this repository. Specifically:

1. Has dark mode been implemented in this frontend project? If not, please indicate that clearly.

2. If dark mode exists, please detail the technical implementation approach:
   - What theming system is being used (CSS variables, styled-components, Tailwind, native Android/iOS theming, etc.)?
   - Is it using a context provider, Redux store, or another state management approach?
   - How are theme preferences persisted (localStorage, UserDefaults, SharedPreferences)?
   - Is there system theme detection (prefers-color-scheme media query or platform APIs)?

3. Analyze the theme switching mechanism:
   - Is it manual toggle, system-based, or both?
   - How are transitions/animations handled when switching themes?
   - Are there any edge cases in the current implementation (Flash of Unstyled Content, etc.)?

4. Evaluate component compatibility:
   - Are all components properly themed or are there inconsistencies?
   - How are third-party components handled with theming?
   - Are there any hardcoded color values that might cause issues?

5. If applicable, identify any accessibility considerations in the dark mode implementation.

Please reference specific files and code examples in your analysis.
```

### Legacy Code Modernization Analysis

```
I need your help analyzing this legacy code repository. Please:

1. Summarize the repository's overall structure, identifying key components and dependencies

2. Extract the main code artifacts including:
   - Primary classes/interfaces
   - Key data structures
   - Important functions/methods
   - Control flow patterns
   - External dependencies

3. Analyze the code quality and modernization potential:
   - Identify outdated programming patterns
   - Note technical debt areas
   - Highlight parts that would benefit from refactoring
   - Suggest modern equivalents for legacy approaches

4. Provide insights on what would be needed to convert this codebase to a more modern implementation:
   - Structural changes required
   - Dependency modernization needs
   - Potential migration challenges
   - Suggested modernization approach

Please be specific and reference actual files/code from this repository in your analysis rather than hypothetical examples.
```

## Tips for Effective Prompting on GitHub.com

1. **Be Specific**: Clearly define what you're looking for
2. **Provide Context**: Mention relevant files or areas of the codebase
3. **Ask Focused Questions**: Break complex analyses into specific questions
4. **Request Structured Output**: Ask for bulleted lists or sections if appropriate
5. **Iterate**: If the first response isn't helpful, refine your prompt

## Limitations to Be Aware Of

- Copilot on GitHub.com may have less context than in your IDE
- Large repositories may be challenging to analyze comprehensively
- The model may not have access to private dependencies or external systems
- Responses are based on the visible code and may miss external factors

## Getting the Most Out of GitHub.com Copilot

- Use it during code reviews to catch issues you might miss
- Generate PR descriptions to save time and improve clarity
- Analyze unfamiliar repositories to quickly understand their structure
- Generate documentation when contributing to open source
- Use it for educational purposes to understand design patterns and architecture

These prompts are starting points - feel free to modify them or combine them to suit your specific needs and projects.
