# Cursor IDE Setup — My First Dev Environment 

## What Is This?
This repository documents my first-ever experience setting up a developer 
environment from scratch — including installing Cursor IDE, AI coding 
extensions, and pushing code to GitHub. I had zero prior experience with 
any of these tools.

## Tools Installed
- **Cursor IDE** - AI-powered code editor built on top of VS Code (https://cursor.com)
- **Claude Code** - Anthropic's AI coding assistant that lives inside your editor
- **Codex** - OpenAI's coding agent extension for writing and reviewing code

## Steps Completed
1. Downloaded and installed Cursor IDE from cursor.com
2. Skipped GitHub connection during Cursor's initial setup (chose "Maybe later")
3. Installed the Claude Code extension from the Extensions marketplace and logged in
4. Installed the Codex extension from the Extensions marketplace and logged in
5. Created a free GitHub account at github.com
6. Created a new public repository called cursor-setup-task with a README file
7. Opened the terminal inside Cursor (Terminal menu → New Terminal)
8. Cloned the repository to my local machine using git clone
9. Opened the cloned folder in Cursor using Open Folder
10. Edited the README.md file with project details
11. Committed and pushed changes to GitHub

## Issues I Ran Into (and How I Solved Them)

### 1. Git wasn't installed on my Mac
Running `git clone` gave an error about missing developer tools. No popup 
appeared either. Fixed it by installing Homebrew, which triggered the 
Xcode Command Line Tools installation automatically.

### 2. Homebrew wasn't in PATH after installing
Even after Homebrew installed, git still didn't work. Had to run two 
commands to add Homebrew to the system PATH before anything worked.

### 3. Ran git clone without the "git clone" prefix
On my first attempt I accidentally pasted just the URL into the terminal 
without the command in front of it. Simple fix once I understood what 
a terminal command actually is.

### 4. Codex login wasn't obvious
There was no visible "Sign In" button. Had to use Cmd+Shift+P and search 
for the Codex command palette option to find the login flow.

### 5. GitHub authentication kept failing
When trying to push, GitHub opened a browser asking for a device code — 
but the code expired before I could enter it. Had to use a Personal Access 
Token (PAT) instead, which required going to GitHub settings to generate one.

### 6. git push got stuck waiting for input
After running git push, the terminal just sat there with a blinking cursor 
and no prompt. Turned out it was waiting for credentials silently. Had to 
use Ctrl+C to cancel and try a different approach.

## What I Learned
- How to use a terminal for the first time
- What git clone actually does (copies a remote repo to your local machine)
- That errors are normal — every issue had a solution
- AI tools like Claude Code and Codex live right inside your code editor
- GitHub no longer accepts passwords — you need a Personal Access Token to push
- How to embed credentials in a git remote URL to bypass authentication prompts
- Ctrl+C is your best friend when the terminal gets stuck

## Time Taken
~45 minutes (mostly troubleshooting git installation)
