# Contributing to GitHub Copilot Workshop

Thank you for your interest in contributing to this workshop! This guide will help you get started.

## 🤝 How to Contribute

### Types of Contributions We Welcome

- **New exercises**: Additional hands-on activities for different skill levels
- **Improved documentation**: Clarifications, corrections, or additional examples
- **New prompting techniques**: Effective patterns you've discovered
- **Language-specific examples**: Examples for different programming languages
- **Bug fixes**: Corrections to existing content or broken links
- **Feature requests**: Ideas for new workshop content

### Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/copilot-workshop.git
   cd copilot-workshop
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```
4. **Create a branch** for your contribution:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Making Changes

#### For Documentation Changes

- Follow the existing Markdown formatting style
- Use consistent heading structure
- Test all code examples
- Run `npm run format:md` to ensure consistent formatting

#### For New Exercises

- Use the template in `.templates/workshop-exercise.template.md`
- Include clear learning objectives
- Provide step-by-step instructions
- Add challenge activities for practice
- Test the exercise yourself

#### For New Prompting Examples

- Add them to `resources/effective-prompts.md`
- Include both effective and less effective examples
- Explain why the prompts work well
- Consider different experience levels

### Code Style & Standards

- Use Prettier for Markdown formatting (`npm run format:md`)
- Follow the existing file naming conventions
- Keep line lengths reasonable (around 100 characters)
- Use semantic line breaks in Markdown
- Include proper attribution for external sources

### Submitting Your Contribution

1. **Test your changes** thoroughly
2. **Commit your changes** with clear, descriptive messages:
   ```bash
   git commit -m "Add exercise for debugging with Copilot Chat"
   ```
3. **Push to your fork**:
   ```bash
   git push origin feature/your-feature-name
   ```
4. **Create a Pull Request** on GitHub with:
   - Clear title describing the change
   - Detailed description of what you've added/changed
   - Context about why the change is beneficial
   - Screenshots if applicable

### Pull Request Guidelines

- Link any related issues
- Ensure all existing exercises still work
- Update the table of contents if you've added new content
- Consider if documentation needs updates
- Be responsive to feedback and requests for changes

## 🎯 Content Guidelines

### Educational Quality

- Content should be beginner-friendly but also valuable for experienced developers
- Include both theory and practical examples
- Provide context for why techniques are useful
- Consider different learning styles

### Inclusivity

- Use inclusive language
- Avoid assumptions about prior knowledge
- Provide multiple approaches when possible
- Consider accessibility in examples

### Technical Accuracy

- Test all code examples
- Verify external links work
- Ensure compatibility with current Copilot features
- Update outdated information

## 📝 Reporting Issues

If you find bugs, have suggestions, or need clarification:

1. **Check existing issues** first to avoid duplicates
2. **Use the appropriate issue template**
3. **Provide clear reproduction steps** for bugs
4. **Include environment details** (IDE, Copilot version, etc.)

## 💡 Getting Help

- **GitHub Discussions**: For questions about using the workshop content
- **Issues**: For bugs or specific improvement suggestions
- **Email**: Reach out to the maintainers for complex discussions

## 🙏 Recognition

All contributors will be recognized in the repository. We appreciate every contribution, whether it's fixing a typo or adding a major new feature!

## 📜 License

By contributing to this project, you agree that your contributions will be licensed under the same MIT License that covers the project.
