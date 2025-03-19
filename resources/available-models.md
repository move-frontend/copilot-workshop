# GitHub Copilot Available Models

GitHub Copilot utilizes different AI models depending on your task, environment, and license tier. Understanding these models can help you select the most appropriate one for your specific needs.

## Model Overview

| Model                       | Strengths                                    | Best For                                           | Availability                  |
| --------------------------- | -------------------------------------------- | -------------------------------------------------- | ----------------------------- |
| **GPT-4o**                  | General-purpose power, nuanced understanding | Complex problems, architectural design             | Free tier and above           |
| **Claude 3.5 Sonnet**       | Speed and accuracy balance                   | Day-to-day coding tasks, explanations              | Free tier and above           |
| **Claude 3.7 Sonnet**       | Advanced reasoning                           | Complex multi-step problems, architecture planning | Business and Enterprise tiers |
| **OpenAI o1**               | Code specialization                          | Programming-specific tasks, optimizations          | Pro tier and above            |
| **OpenAI o3-mini**          | Speed                                        | Simpler tasks, quick completions                   | Free tier and above           |
| **Google Gemini 2.0 Flash** | Efficiency                                   | Fast responses to straightforward queries          | Free tier and above           |

## Where to Select Models

The ability to select models varies by environment:

### VS Code / IDE Copilot Chat

In VS Code and other IDEs, you can select your preferred model from the dropdown menu at the top of the Copilot Chat panel:

![Model selection dropdown in VS Code](https://example.com/model-selection.png)

### GitHub.com

On GitHub.com, Copilot automatically selects the appropriate model for your interaction, so no manual selection is required.

## Feature Availability by Model

Not all models support all features. Here's a breakdown:

| Feature                  | GPT-4o  | Claude 3.5 Sonnet | Claude 3.7 Sonnet | OpenAI o1 |
| ------------------------ | ------- | ----------------- | ----------------- | --------- |
| Code Completions         | ✓       | ✓                 | ✓                 | ✓         |
| Code Explanations        | ✓       | ✓                 | ✓                 | ✓         |
| Multi-turn Conversations | ✓       | ✓                 | ✓                 | ✓         |
| Agent Mode               | Limited | Limited           | ✓                 | Limited   |
| Repository Analysis      | ✓       | ✓                 | ✓                 | ✓         |
| Code Review              | ✓       | ✓                 | ✓                 | ✓         |
| Documentation Generation | ✓       | ✓                 | ✓                 | ✓         |

## When to Use Each Model

### GPT-4o

- Complex problem solving requiring broad context understanding
- Nuanced code explanations that relate to business logic
- Tasks requiring understanding of both code and natural language

### Claude 3.5 Sonnet

- Everyday coding assistance
- Clear, concise explanations
- Well-balanced performance for most tasks

### Claude 3.7 Sonnet

- Complex architectural decisions
- Multi-step reasoning tasks
- Advanced problem decomposition
- Projects requiring consistent context awareness across a conversation

### OpenAI o1

- Highly specialized coding tasks
- Performance optimization suggestions
- Technical documentation generation

### Smaller Models (o3-mini, Gemini 2.0 Flash)

- Simple code completions
- Basic explanations
- When speed is more important than depth

## Best Practices for Model Selection

1. **Start with the default** - In most cases, the default model will be sufficient
2. **Switch for complex tasks** - Move to Claude 3.7 Sonnet or GPT-4o for architecture planning
3. **Consider performance** - Use lighter models when responsiveness is critical
4. **Match to task** - Technical code tasks → o1, Reasoning tasks → Claude 3.7 Sonnet
5. **Experiment** - Try different models on the same prompt to compare outputs

## License Tier Considerations

Your access to models depends on your GitHub Copilot license tier:

- **Free**: Limited access to base models
- **Pro**: Access to all models except those exclusive to Business/Enterprise
- **Business**: Full access to all models including Claude 3.7 Sonnet
- **Enterprise**: Full access plus preview features and organizational knowledge base integration

## Note on Future Updates

GitHub Copilot's available models are regularly updated as AI technology evolves. This document reflects the state as of March 2025, but new and improved models may be added over time.
