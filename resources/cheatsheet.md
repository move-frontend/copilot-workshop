# GitHub Copilot Cheatsheet

This quick reference guide covers the most common GitHub Copilot commands, shortcuts, and usage patterns to help you maximize your productivity.

## Keyboard Shortcuts

### Code Completions

| Action                         | Windows/Linux | macOS       |
| ------------------------------ | ------------- | ----------- |
| Accept suggestion              | `Tab`         | `Tab`       |
| Dismiss suggestion             | `Esc`         | `Esc`       |
| Show next suggestion           | `Alt+]`       | `Option+]`  |
| Show previous suggestion       | `Alt+[`       | `Option+[`  |
| Trigger inline completions     | `Alt+\`       | `Option+\`  |
| Open Copilot completions panel | `Ctrl+Enter`  | `Cmd+Enter` |

### Copilot Chat

| Action                          | Windows/Linux         | macOS                 |
| ------------------------------- | --------------------- | --------------------- |
| Open Copilot Chat               | `Ctrl+Alt+I`          | `Cmd+Option+I`        |
| Focus on Chat input             | `Ctrl+Alt+/`          | `Cmd+Option+/`        |
| Insert code from Chat to editor | Click "Insert" button | Click "Insert" button |

## Chat Commands

| Command     | Description                      | Example                     |
| ----------- | -------------------------------- | --------------------------- |
| `/explain`  | Explain selected code            | `/explain [selected code]`  |
| `/tests`    | Generate tests for selected code | `/tests [selected code]`    |
| `/fix`      | Fix issues in selected code      | `/fix [problematic code]`   |
| `/doc`      | Generate documentation           | `/doc [selected function]`  |
| `/optimize` | Optimize selected code           | `/optimize [selected code]` |
| `/new`      | Start a new chat                 | `/new`                      |
| `/clear`    | Clear current chat               | `/clear`                    |

## Effective Prompting Patterns

### For Code Completions

1. **Be specific with comments**:

   ```javascript
   // Create a function that validates email using regex and returns true/false
   ```

2. **Provide function signatures**:

   ```javascript
   /**
    * @param {string[]} items - Array of strings to filter
    * @param {string} searchTerm - The term to search for
    * @returns {string[]} - Filtered array
    */
   function filterItems(items, searchTerm) {
   ```

3. **Include expected output format**:
   ```javascript
   // Format the date (2023-03-15) as "March 15, 2023"
   ```

### For Copilot Chat

1. **Specify language and framework**:

   ```
   How do I implement form validation in React using Formik?
   ```

2. **Include error messages and context**:

   ```
   I'm getting this error: "Cannot read property 'map' of undefined".
   Here's my component code:
   [code snippet]
   ```

3. **Ask for step-by-step guidance**:
   ```
   Can you walk me through implementing JWT authentication in an Express app step by step?
   ```

## GitHub Web Integration

| Feature           | How to Access                                             |
| ----------------- | --------------------------------------------------------- |
| PR Description    | Look for "Generate description" button when creating a PR |
| Code Explanations | Select code in GitHub.com and look for Copilot icon       |
| Issue Summaries   | Look for Copilot icon in issue description field          |
| PR Reviews        | Type "@copilot" in a review comment                       |

## Model Selection

Different models have different strengths. When available, you can select between:

| Model             | Best For                                            |
| ----------------- | --------------------------------------------------- |
| GPT-4o            | Complex problem-solving, nuanced code understanding |
| Claude 3.5 Sonnet | Well-balanced for most coding tasks                 |
| Claude 3.7 Sonnet | Advanced reasoning (Business/Enterprise tiers)      |
| OpenAI o1         | Specialized code capabilities (Pro tier+)           |

## Troubleshooting

1. **Not seeing suggestions?**

   - Check Copilot status in editor status bar
   - Ensure you've signed in with a licensed account
   - Try typing a more specific comment

2. **Suggestions not relevant?**

   - Provide more context in comments
   - Open relevant files to give Copilot more context
   - Try breaking down complex tasks into smaller steps

3. **Chat not working?**
   - Verify you have Copilot Chat extension installed
   - Check that your subscription tier includes Chat access
   - Try restarting your IDE

## License Tier Features

| Feature          | Free        | Pro | Business | Enterprise |
| ---------------- | ----------- | --- | -------- | ---------- |
| Code Completions | ✓ (Limited) | ✓   | ✓        | ✓          |
| Copilot Chat     | ✓ (Limited) | ✓   | ✓        | ✓          |
| Agent Mode       | ❌          | ❌  | ✓        | ✓          |
| Web Integration  | ✓           | ✓   | ✓        | ✓          |
| Advanced Models  | ❌          | ✓   | ✓        | ✓          |
| Knowledge Base   | ❌          | ❌  | ❌       | ✓          |
