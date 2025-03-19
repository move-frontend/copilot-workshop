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
2. In comment fields or descriptions, type `@copilot` followed by your prompt
3. Wait for Copilot to generate a response
4. Review and use the insights provided

## Repository Analysis Prompts

### Code Understanding

```
@copilot Explain the architecture of this repository and how the main components interact with each other.
```

```
@copilot Summarize what this file does and how it fits into the larger codebase.
```

```
@copilot What design patterns are being used in this repository?
```

```
@copilot Identify the key classes/functions in this repository and explain their responsibilities.
```

### Code Quality Analysis

```
@copilot Review this code for potential performance issues or bottlenecks.
```

```
@copilot Identify any security vulnerabilities in this repository, particularly around user authentication.
```

```
@copilot What parts of this codebase would benefit most from refactoring?
```

```
@copilot Analyze the complexity of this code and suggest simplifications.
```

## Pull Request Enhancement

### Description Generation

```
@copilot Generate a comprehensive description for this pull request that explains the changes and their purpose.
```

```
@copilot Create a structured PR description that includes background, changes made, testing performed, and potential impacts.
```

### Testing Suggestions

```
@copilot Suggest tests that should be added to cover the changes in this pull request.
```

```
@copilot What edge cases should be considered when testing these changes?
```

### Impact Analysis

```
@copilot What potential impacts might these changes have on other parts of the codebase?
```

```
@copilot Are there any performance implications from these changes that should be noted?
```

## Documentation Generation

### Repository Documentation

```
@copilot Create a README for this repository that explains its purpose, installation steps, and usage examples.
```

```
@copilot Generate a CONTRIBUTING.md file that explains how to contribute to this project.
```

### Code Documentation

```
@copilot Generate JSDoc comments for this function that explain parameters, return values, and examples.
```

```
@copilot Create documentation for this API endpoint including parameters, response format, and error handling.
```

## Project Management

### Issue Analysis

```
@copilot Based on the issues and PRs, what are the main areas of active development in this repository?
```

```
@copilot Suggest a roadmap for this project based on existing issues and pull requests.
```

### Dependency Management

```
@copilot What dependencies in this project are outdated and should be updated?
```

```
@copilot Analyze the dependencies in this project and identify any that might pose security or compatibility risks.
```

```
@copilot Are there any unused dependencies that could be removed from this project?
```

## Code Review Assistance

### Review Comments

```
@copilot What code standards or conventions are not being followed in this PR?
```

```
@copilot Is this implementation consistent with similar features in the codebase?
```

```
@copilot Suggest ways to make this code more maintainable and readable.
```

### Best Practices

```
@copilot How could this code be improved to follow modern best practices?
```

```
@copilot Are there any potential memory leaks or resource management issues in this code?
```

## Test Coverage Analysis

```
@copilot What areas of the codebase appear to lack test coverage?
```

```
@copilot Generate unit tests for this component that cover the main functionality and edge cases.
```

```
@copilot How could we improve the existing test suite for better coverage?
```

## Performance and Optimization

```
@copilot Identify any N+1 query issues in this repository's database access code.
```

```
@copilot Are there opportunities to implement caching to improve performance in this codebase?
```

```
@copilot Suggest ways to optimize the frontend bundle size based on the configuration files.
```

## Issue Templates

```
@copilot Create a detailed issue template for bug reports that would be appropriate for this repository.
```

```
@copilot Generate a feature request template that captures requirements and acceptance criteria.
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
