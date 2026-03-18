# Bulk Repository Management

These scripts exist to automate repository management, en massé. The goal is that you never have to touch the terminal when developing with Git.

## Scripts

### [`mass-pull`](/shell/git/mass/mass-pull)

Automatically pull **all repos** in **all authors** in your `~/GitHub/` folder.

#### Usage

Run the script from the parent directory containing your Git author folders:

```bash
./all-push
```

### [`new-repo`](/shell/git/mass/new-repo)

Automate the whole process of creating a repository locally and on GitHub.

Requires `git`, `gh` and `ssh`.

#### Usage

Just run the `new-repo` script:

```bash
bash new-repo
```

The script will guide you through the process.

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
