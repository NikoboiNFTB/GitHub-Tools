# Single Repository Management

These scripts exist to automate single repository management. The goal is that you never have to touch the terminal when developing with Git.

## Scripts

### [`pull`](/shell/git/repo/pull)

Pulls the latest changes for the current Git repository.

#### Usage

Save the script to a folder called `automation` in your git repository. Add `/automation/` as an entry to `/.git/info/exclude/`. Then run it from either the automation folder or the repository folder.

```bash
user@pc:~/GitHub/NikoboiNFTB/GitHub-Tools$ bash automation/pull
```

or

```bash
user@pc:~/GitHub/NikoboiNFTB/GitHub-Tools/automation$ bash pull
```

> > `..` means parent directory

### [`push`](/shell/git/repo/push)

Stage, commit, and push changes for the current repository. Supports custom commit message.

#### Usage

Save the script to a folder called `automation` in your git repository. Add `/automation/` as an entry to `/.git/info/exclude/`. Then run it from either the automation folder or the repository folder.

```bash
user@pc:~/GitHub/NikoboiNFTB/GitHub-Tools$ bash automation/pull
```

or

```bash
user@pc:~/GitHub/NikoboiNFTB/GitHub-Tools/automation$ bash push
```

> > `..` means parent directory

### [`status`](/shell/git/repo/status)

Displays the current `git status` for all repositories in subdirectories, showing staged and unstaged changes for each.

#### Usage

Save the script to a folder called `automation` in your git repository. Add `/automation/` as an entry to `/.git/info/exclude/`. Then run it from either the automation folder or the repository folder.

```bash
user@pc:~/GitHub/NikoboiNFTB/GitHub-Tools$ bash automation/pull
```

or

```bash
user@pc:~/GitHub/NikoboiNFTB/GitHub-Tools/automation$ bash status
```

> > `..` means parent directory

## Installation

You can grab any one of the scripts into any folder simply by running:

```bash
wget https://github.nikoboi.dev/shell/*
```

> > Fill in the path to the script. [github.nikoboi.dev](https://github.nikoboi.dev/) resolves to this repository.

Or run the automation setup script. Run anywhere (the script self-corrects using `$HOME`, `mkdir -p` and `cd`):

```bash
bash <(wget -qO- https://github.nikoboi.dev/shell/setup/automation)
```

The `automation` setup script also works as an update script.

> > Will setup my entire automation workflow. See the [file tree](/README.md#file-tree) for details.
