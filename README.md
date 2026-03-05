GitMan - Git Manager
====================
A simple Unix shell script GUI to manage pulling and pushing multiple repos at once.

## Installation

1. Make the script executable:
```bash
chmod +x gitman
```

2. Move to your PATH (optional):
```bash
sudo mv gitman /usr/local/bin/
```

3. Install dialog if needed:
```bash
sudo apt install dialog    # Debian/Ubuntu
sudo yum install dialog    # RHEL/CentOS
```

## Usage

Run without arguments to open the interactive menu:
```bash
./gitman                   # or just 'gitman' if in PATH
```

Navigate the menu with arrow keys and Enter:

- **Add repository**: Register a repo by providing a name and path
- **List repositories**: View all registered repos
- **Remove repository**: Unregister a repo from the list
- **Pull all repositories**: Run `git pull` on all registered repos
- **Push all repositories**: Run `git push` on all registered repos

## CLI Options

```bash
gitman --help                            # Show help
gitman --list                            # List all registered repos
gitman --pull                            # Pull all registered repos
gitman --push                            # Push all registered repos
gitman --repo add <name> </path>         # Register a repo
gitman --repo remove <name>              # Unregister a repo
```

## Config File

The registry is stored at `~/.git_man/.repo_registry` with one entry per line.
The format is `<name>:<file_path>`.
