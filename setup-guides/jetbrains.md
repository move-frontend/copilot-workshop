# Setting Up GitHub Copilot in JetBrains IDEs

This guide provides basic steps to get GitHub Copilot up and running in JetBrains IDEs like IntelliJ with your GitHub Copilot Business license.

## Prerequisites

- [JetBrains IntelliJ IDEA](https://www.jetbrains.com/idea/) installed on your machine (or any other JetBrains IDE)
- Your GitHub account with access to GitHub Copilot Business
- Organization membership with Copilot Business enabled

## Installation Steps

### Automated Setup (Recommended)

1. Open IntelliJ IDEA
2. Go to **File > Settings** (or **IntelliJ IDEA > Preferences** on macOS)
3. Navigate to **Plugins** and search for "GitHub Copilot"
4. Click **Install** to install the GitHub Copilot plugin
5. Restart IntelliJ IDEA to activate the plugin
6. After restarting, you will be prompted to sign in to GitHub
7. Complete the authentication process in your browser
8. If prompted, select the GitHub account associated with your Business license

### Manual Setup (Alternative)

1. Open IntelliJ IDEA
2. Go to **File > Settings** (or **IntelliJ IDEA > Preferences** on macOS)
3. Navigate to **Plugins** and click on the **Marketplace** tab
4. Search for "GitHub Copilot" and install the plugin
5. Restart IntelliJ IDEA to activate the plugin
6. After restarting, open the **Tools** menu and select **GitHub Copilot: Sign In**
7. Follow the authentication steps in your browser

## Verifying the Installation

After installation, you can verify Copilot Business is working by:

1. Opening a code file and typing a comment to see if code suggestions appear
2. Checking that the Copilot status in the bottom bar shows "Ready"

## Switching GitHub Accounts

If you need to use a different GitHub account with Copilot:

1. Go to **File > Settings** (or **IntelliJ IDEA > Preferences** on macOS)
2. Navigate to **Appearance & Behavior > System Settings > Passwords**
3. Remove the existing GitHub account credentials
4. Restart IntelliJ IDEA
5. Sign in with your alternative GitHub account that has Copilot access

## Useful Keyboard Shortcuts

- Accept code suggestion: `Tab`
- Dismiss code suggestion: `Esc`
- Show next suggestion: `Alt+]` / `Option+]`
- Show previous suggestion: `Alt+[` / `Option+[`

## Additional Resources

- [Official JetBrains Copilot Setup Guide](https://docs.github.com/en/copilot/using-github-copilot/getting-code-suggestions-in-your-ide-with-github-copilot?tool=jetbrains)
- [GitHub Copilot Quickstart](https://docs.github.com/en/copilot/getting-started-with-github-copilot)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [GitHub Copilot Cheat Sheet](https://docs.github.com/en/copilot/getting-started-with-github-copilot/cheat-sheet)

---

_Note: GitHub Copilot is continuously being updated with new features. For the most current setup instructions, refer to the official documentation._
