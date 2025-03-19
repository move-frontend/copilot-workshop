# Dependabot Exercise

## Overview

Learn to automate dependency management using GitHub Copilot and Dependabot to eliminate manual checks, improve security, and save time for what really matters.

## Learning Objectives

- Objective 1: Using GitHub Copilot Chat to create Dependabot configurations
- Objective 2: Understanding how Dependabot helps automate dependency management
- Objective 3: Applying custom configurations to address specific project needs

## Prerequisites

- GitHub Copilot and Copilot Chat enabled in your IDE
- Access to a GitHub repository where you can add Dependabot configuration
- Basic knowledge of package managers (npm, pip, composer, etc.)

## Exercise Steps

### Step 1: Understand the Problem with Manual Dependency Audits

1. Review the common manual approaches to dependency management. This often includes a command or Bash script that runs periodically. Here are a few examples of such commands:

```bash
# Node.js
$ npm outdated

# Python
$ pip list --outdated

# PHP
$ composer outdated
```

2. Consider the limitations of manual dependency checks:
   - Time-consuming
   - Easily forgotten
   - No automatic security vulnerability detection

### Step 2: Enable Dependabot for Outdated Dependencies

Use GitHub Copilot to configure Dependabot to automatically create pull requests for outdated packages.

> An example prompt could be: `Create a minimal Dependabot configuration to get started for my npm packages`. Copilot will generate a configuration file for you.

> 💡 **Tip:** The generated configuration could look similar to this:

```yaml
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "weekly"
```

### Step 3: Customize the Configuration

You can also use GitHub Copilot to add more features to your Dependabot configuration. For example, you can set the schedule to daily or monthly, or even specify a custom time. You can also configure it to ignore certain dependencies or automatically assign reviewers to the pull requests.

> An example prompt could be: `I want my dependency updates at 8am on Mondays using Amsterdam timezone, with a limit of 10 open pull requests. Use the integration branch 'integration/dependabot' as the target and automatically assign the label 'dependencies' and a reviewer.`

> 💡 **Tip:** The generated configuration could look similar to this:

```yaml
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "weekly"
      day: "monday"
      time: "08:00"
      timezone: "Europe/Amsterdam"
    open-pull-requests-limit: 10
    target-branch: "integration/dependabot"
    labels:
      - "dependencies"
    reviewers:
      - "octocat"  # Replace with actual GitHub username
```

Modify the suggested configuration as needed for your project

### Step 4: Explore Additional Configuration Options

You can further customize the configuration to suit your needs. Ask Copilot what other options are available or add another package ecosystem to the configuration.

## Challenge Activities

Now that you've learned the basics, try these challenges on your own:

### Challenge 1: Multi-Ecosystem Configuration

Create a configuration that handles dependencies for two different ecosystems (e.g., npm, Docker and Github Actions). Consider how to configure each with different schedules.

### Challenge 2: Advanced Configuration

Create a more complex setup with ignore rules for certain dependencies, grouped dependencies, custom commit messages, and version strategy settings.

## Tips for Success

- Be specific about which package ecosystem you're using for better suggestions
- Consider configuring different update schedules for different dependency types
- Remember that Dependabot configurations can be tested in incremental steps
- Combine Copilot's suggestions with the Dependabot documentation for best results

## Next Steps

Once you've completed this exercise, you can:

- Implement the Dependabot configuration in your own repositories
- Explore how to effectively review and manage Dependabot pull requests
- Try applying what you've learned to automate other maintenance tasks

## Sources

For the most current and detailed information, please refer to these official resources:

- [GitHub Copilot - How to run dependency audits with GitHub Copilot](https://github.blog/developer-skills/github/video-how-to-run-dependency-audits-with-github-copilot/)
- [Dependabot options reference](https://docs.github.com/en/code-security/dependabot/working-with-dependabot/dependabot-options-reference)
