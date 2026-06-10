# Cursor IDE Setup

## Tools Installed

1. Cursor IDE (v3.7.21)
2. Claude Code Extension
3. Codex Extension
4. Git
5. GitHub

## Steps Completed

### Step 01: Install Cursor IDE
Cursor IDE was downloaded from the official website (https://cursor.com). The Windows x64 User Installer was selected, as the system runs a 64-bit version of Windows. After installation, the version was confirmed as Cursor 3.7.21. The application was then opened and signed in using a Google account.

### Step 02: Locate the Extensions Panel
According to the setup instructions, the next step was to navigate to Extensions → Search "Claude Code". However, Cursor opened in the "Agent Interface" instead of the "Editor Interface", so no Extensions icon or panel was visible in the sidebar. Exploring the "Customize" option revealed a Marketplace, but searching for Claude Code or Codex returned no relevant results. By exploring all icons and options within the Agent Interface, an icon at the top was found to navigate to the "Editor Interface", where Extensions are available under the "View" menu.

### Step 03: Install Claude Code and Log In
Extensions → Search "Claude Code" was performed. The Claude Code extension by Anthropic was already installed. The option "Claude Code: Open in Sidebar" was used to log in, and the terminal displayed the Claude environment, confirming that Claude Code was successfully installed and authenticated.

### Step 04: Install Codex and Log In
Similarly, Extensions → Search "Codex" was performed. The Codex extension by OpenAI was already installed. The option "Codex: Open Codex Sidebar" was used to log in, and the terminal displayed the ChatGPT environment, confirming successful installation and authentication.

### Step 05: Verify Installed Extensions
The following command was run in the Cursor PowerShell terminal:
 "cursor --list-extensions"

Output:

 "anthropic.claude-code" 
 
 "anysphere.remote-ssh"
 
 "openai.chatgpt"

This output confirmed that both required extensions were installed successfully.

### Step 06: Create GitHub Repository
A GitHub repository named "100Hires-cursor-setup" was created with visibility set to Public. The repository was cloned locally using "git clone"and then opened in Cursor IDE.

Repository URL: https://github.com/Renu1213/100Hires-cursor-setup

### Step 07: Create README File
With the project folder (repository: 100Hires-cursor-setup) open in Cursor, a new file was created using the "New File" option in the left file explorer. The file was named "README.md", populated with the Cursor setup details, and saved successfully.

### Step 08: Commit and Push Changes to GitHub
After creating the README file, a local Git repository was initialized and connected to the GitHub repository. The README file was then staged, committed, and pushed to the main branch.
The following commands were used:

 "git init"
 
 "git remote add origin https://github.com/Renu1213/100Hires-cursor-setup.git"
 
 "git branch -M main"
 
 "git add README.md"
 
 "git commit -m "Initial README setup" "
 
 "git push -u origin main"
 

GitHub authentication was completed through the browser when prompted, and the repository was successfully synchronized with GitHub.

## Issues Faced and How They Were Solved

Issue 01

ISSUE: After logging in, Cursor launched in its modern Agent Interface by default. This interface has a different layout from the traditional editor view, and no Extensions icon or panel appeared in the sidebar. The sidebar displayed only Agent-mode navigation options. Exploring the Customize section revealed a Marketplace, but searching for Claude Code or Codex returned no relevant results.

SOLVED BY: By exploring all icons and options within the Agent Interface, an icon at the top was identified as the navigation point to the Editor Interface, where the Extensions panel is available under the View menu.

Issue 02

ISSUE: Searching for extensions within the application returned results such as "Start Extension Host CPU Profiler," "Start Extension Host Heap Allocator Profiler," and "Start Extension Host RPC Profiler." These were internal developer debugging tools, not extension installation options.

SOLVED BY: These results were identified as unrelated to extension installation. The search approach was abandoned, and alternative methods for installing the required extensions were explored.

Issue 03

ISSUE: The required extensions were not available through the Marketplace interface. Searching the Marketplace for "Claude Code" returned no relevant results.

SOLVED BY: The extensions were installed directly using the Cursor CLI with the following commands:
 
 "cursor --install-extension anthropic.claude-code" 

 "cursor --install-extension openai.chatgpt" 

Issue 04

ISSUE: After the Claude Code and Codex extensions were installed, no visible login prompt or sign-in button appeared within the extensions.

SOLVED BY: The options "Claude Code: Open in Sidebar" and "Codex: Open Codex Sidebar" were used to initiate authentication. The terminal subsequently displayed the Claude environment and ChatGPT environment respectively, confirming that both extensions were successfully installed and authenticated.


The Cursor IDE was successfully installed and configured with Claude Code and Codex extensions.
