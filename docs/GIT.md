> [!WARNING]
> Not updated.

# Git Scripts

Powerful scripts for `git`.

## [`clone`](/git/clone)

Will clone one or all repositories of a specified author, using either HTTPS or SSH.

### Usage

```bash
clone [METHOD] [AUTHOR] [REPO]
```

Arguments are positional and interpreted in this order:

1. `METHOD` — `https` or `ssh`

2. `AUTHOR` — GitHub username or organization

3. `REPO` — Repository name, or `ALL` to clone all repositories

All arguments are optional. If any are missing, the script will prompt for them interactively.

If `REPO` is omitted or left empty when prompted, it defaults to `ALL` (clone all repositories for the given author).

#### Examples

```bash
clone https torvalds linux         # Clone a specific repository using HTTPS.
clone https linuxmint ALL          # Clone all repositories from a user or organization.
clone ssh NikoboiNFTB GitHub-Tools # Clone a specific repository using SSH.
clone                              # Fully interactive mode (you will be prompted for all inputs).
```

## [`pull`](/git/pull)

Pulls all remote changes to one or more repositories.

### Usage

Just run `pull` in any folder. The script will seek out all repositories in all subfolders using `find . -name ".git"` and then extrapolating the repository path from that.

#### Examples

```bash
~/
```

## [`push`](/git/push)

blahblah

## [`status`](/git/status)

blahblah

## [`toggle-ssh`](/git/toggle-ssh)
