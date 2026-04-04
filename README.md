> [!WARNING]
> [`/docs/`](/docs/) are not updated.

# GitHub-Tools

A collection of Shell Scripts for Git and userscripts for GitHub.

Each tool exists to make repetitive Git tasks a little less tedious.

## Table of Contents

Each entry can be clicked for a detailed description of each script.

### Shell

| Script                          | Description                   | README                            |
| ------------------------------- | ----------------------------- | --------------------------------- |
| [`clone`](/git/clone)           | Clone repos of any author     | [GIT.md](/docs/GIT.md#clone)      |
| [`pull`](/git/pull)             | Pull remote changes for repos | [GIT.md](/docs/GIT.md#pull)       |
| [`push`](/git/push)             | Push local changes for repos  | [GIT.md](/docs/GIT.md#push)       |
| [`status`](/git/status)         | View Status of repos          | [GIT.md](/docs/GIT.md#status)     |
| [`toggle-ssh`](/git/toggle-ssh) | Enable your SSH key           | [GIT.md](/docs/GIT.md#toggle-ssh) |

### Userscript

| Script                                                             | Description                                                        | README                                     | Install                                                                                                        |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
| [`auto-reload.user.js`](/userscript/auto-reload.user.js)           | Automatically reloads your GitHub repo if it's pending deployment. | [USER.JS.md](/docs/USER.JS.md#auto-reload) | [install](https://github.com/NikoboiNFTB/GitHub-Tools/raw/refs/heads/main/userscript/auto-reload.user.js)      |
| [`delete-full-auto.user.js`](/userscript/delete-full-auto.user.js) | Automatically fills in all repo deletion steps.                    | [USER.JS.md](/docs/USER.JS.md#full-auto)   | [install](https://github.com/NikoboiNFTB/GitHub-Tools/raw/refs/heads/main/userscript/delete-full-auto.user.js) |
| [`delete-semi-auto.user.js`](/userscript/delete-semi-auto.user.js) | Automatically fills in the text repo deletion step.                | [USER.JS.md](/docs/USER.JS.md#semi-auto)   | [install](https://github.com/NikoboiNFTB/GitHub-Tools/raw/refs/heads/main/userscript/delete-semi-auto.user.js) |

## Installation

You can grab any one of the scripts into any folder simply by running:

```bash
wget https://github.nikoboi.dev/git/*
```

> > Fill in the path to the script. [github.nikoboi.dev](https://github.nikoboi.dev/) resolves to this repository.

Or run the automation setup script. Run anywhere (the script self-corrects using `$HOME`, `mkdir -p` and `cd`):

```bash
bash <(wget -qO- https://github.nikoboi.dev/shell/setup/automation)
```

The `automation` setup script also works as an update script.

> > Will setup my entire automation workflow. All scripts will be installed to `/usr/local/bin/`.

## Contributing

Feel free to fork this repository and submit issues or pull requests if you have any suggestions or improvements. If you encounter any bugs or have feature requests, please open an issue.

## Credits

Created by [**Nikoboi**](https://github.com/NikoboiNFTB/)

Script logic fine-tuned using [**ChatGPT**](https://chatgpt.com/)

## License

This project is licensed under the GNU General Public License V3. See [LICENSE](/LICENSE) for details.
