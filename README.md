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

Run the script:
```bash
./gitman                   # or just 'gitman' if in PATH
```

Navigate the menu with arrow keys and Enter:

- **Add repository**: Register a repo by providing a name and path
- **List repositories**: View all registered repos
- **Remove repository**: Unregister a repo from the list
- **Pull all repositories**: Run `git pull` on all registered repos
- **Push all repositories**: Run `git push` on all registered repos

Registry stored in `~/.git_man/.repo_registry`
