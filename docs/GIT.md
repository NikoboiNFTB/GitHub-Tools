# Git Scripts

Powerful scripts for `git`. All scripts should be saved into `/usr/local/bin/`.

## [`clone`](/git/clone)

Will clone one or all repositories of a specified author, using either HTTPS or SSH.

### Clone Usage

```bash
clone [METHOD] [AUTHOR] [REPO]
```

Arguments are positional and interpreted in this order:

1. `METHOD` — `https` or `ssh`

2. `AUTHOR` — GitHub username or organization

3. `REPO` — Repository name, or `ALL` to clone all repositories

All arguments are optional. If any are missing, the script will prompt for them interactively.

If `REPO` is omitted or left empty when prompted, it defaults to `ALL` (clone all repositories for the given author).

#### Clone Examples

```bash
clone https torvalds linux         # Clone a specific repository using HTTPS.

clone https linuxmint ALL          # Clone all repositories from a user or organization.

clone ssh NikoboiNFTB GitHub-Tools # Clone a specific repository using SSH.

clone                              # Fully interactive mode (you will be prompted for all inputs).
```

## [`pull`](/git/pull)

Pulls all remote changes to one or more local repositories.

### Pull Usage

Just run `pull` in any folder.

The script will seek out all repositories in all subfolders using `find . -name ".git"` and then extrapolating the repository path from that.

#### Pull Examples

```bash
~/GitHub/NikoboiNFTB/GitHub-Tools$ pull

~/GitHub/NikoboiNFTB$ pull

~/GitHub$ pull
```

## [`push`](/git/push)

Pushes all local changes to one or more remote repositories.

### Push Usage

Just run `push` in any folder. A commit comment can be added as an argument in quotations, or submit when prompted.

The script will seek out all repositories in all subfolders using `find . -name ".git"` and then extrapolating the repository path from that.

#### Push Examples

```bash
~/GitHub/NikoboiNFTB/GitHub-Tools$ push "Change feature x"

~/GitHub/NikoboiNFTB$ push
Enter commit message (Enter to use 'Update'): Mass update.

~/GitHub$ push "This will not work for some repos because not owner"
```

## [`status`](/git/status)

Runs `git add .` and `git status`. Works same as `pull` and `push`.

## [`toggle-ssh`](/git/toggle-ssh)

Toggles SSH for GitHub. Requires SSH key to be saved as `~/.ssh/id_ed25519_github` and `~/.ssh/id_ed25519_github.pub`. Will move both keys to `~/.ssh.bak/` and remote them using `ssh-add -d`.
