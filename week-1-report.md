## Connor Wu - Week 1 Lab Report: Remote Access Tutorial

### Step 1: Download Visual Studio Code

Start by downloading [Visual Studio Code](https://code.visualstudio.com/) for your respective operating system and follow the setup instructions.
It should look something like this upon opening the software:
![image](assets/report-1/vscode.PNG)

### Step 2: Download Git

Download and install [Git For Windows](https://gitforwindows.org/)
This will be used to access Git Bash, which contains useful command-line tools for git repositories and remote access.

### Step 3: Configure Git Bash in VSCode

1. Open the command palette in VSCode using Ctrl+Shift+P
2. Type `Terminal: Set Default Profile`
3. From the drop-down menu, select Git Bash:
   ![image](assets/report-1/commandpalette.png)
4. Open the Terminal: Terminal --> New Terminal or Ctrl+`

### Step 4: SSH into the server

Use this command but with your specific username to access the remote server:
`$ ssh cs15lwi23zz@ieng6.ucsd.edu`
