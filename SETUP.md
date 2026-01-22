# Setup — Install Git and publish to GitHub

Follow these steps before starting the exercise.
Use a terminal (Terminal on macOS/Linux, PowerShell or Git Bash on Windows) for the commands below.

## 1) Install Git

- Windows
  - Download "Git for Windows" from [git-scm.com/download/win](https://git-scm.com/download/win)
  - Run the installer and accept the defaults
  - After install, open PowerShell or Git Bash and verify:
    - `git --version`

- macOS
  - EITHER install Xcode Command Line Tools: `xcode-select --install`
  - OR use Homebrew: `brew install git`
  - Verify: `git --version`

- Linux (Ubuntu/Debian)
  - `sudo apt update && sudo apt install -y git`
  - Verify: `git --version`

- Linux (Fedora)
  - `sudo dnf install -y git`
  - Verify: `git --version`

## 2) Configure your Git identity (once)

Run these commands in a terminal, replacing with your info:

- `git config --global user.name "Your Name"`
- `git config --global user.email "you@example.com"`
- Optional (recommended): `git config --global init.defaultBranch main`

You can view settings with:

- `git config --list --global`

## 3) Create a GitHub account and sign in when prompted

- Create an account: [github.com/join](https://github.com/join)
- When you push from the terminal the first time, a sign-in prompt (Git Credential Manager) may appear. Sign in with your GitHub account in the browser window that opens.



## 4) Students — Fork and clone (recommended workflow)

1) Open your teacher's repository on GitHub
2) Click "Fork" to create your copy under your account
3) Clone your fork to your computer:
   - On GitHub, click the green "Code" button and copy the HTTPS URL
   - In a terminal: `git clone https://github.com/<your-username>/<repo>.git`
4) Change into the folder: `cd <repo>`
5) Confirm you are on `main`: `git branch --show-current`

You are ready to start the tasks in [README.md](README.md).

## Troubleshooting

- Authentication prompt keeps asking for credentials
  - Make sure a browser window opened to sign in; complete the flow
  - On Windows, Git for Windows installs Git Credential Manager (GCM) by default
- "Permission denied" when pushing
  - Confirm the remote URL points to YOUR fork: `git remote -v`
  - If not, update it: `git remote set-url origin https://github.com/<your-username>/<repo>.git`
- Name or email incorrect on commits
  - Update with `git config --global user.name` and `git config --global user.email`
