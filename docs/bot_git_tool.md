---
layout: page
title: Bot GIT Tool
permalink: /bot_git_tool
---

<br>
<br>

# Bot GIT Tool

### A collection of Bash script tools made to simplify and speed up your GIT workflow automation.

- GIT List

  This application efficiently identifies all repositories located within the specified directories, offering a
  comprehensive overview of your projects. GIT List also appends the git path to the '.gitconfig' file.

<br>
<br>

# 🪧 Usage

Clone the [Bot GIT Tool][bot_git_tool] repository anywhere you want 'bot_git_tool' on your system.

```
git clone --recurse-submodules https://github.com/iamprogrammerlk/bot_git_tool.git
```

> [!IMPORTANT]
>
> Don't forget the `--recurse-submodules` option,

If you already cloned the project and forgot `--recurse-submodules`, You must run following two commands from
the main project `git submodule init` to initialize your local configuration file, and `git submodule update` to
fetch all the files from the `bot_git_tool` project, you can use the foolproof
`git submodule update --init --recursive` command to also initialize, fetch and checkout any nested submodules.

## GIT List

This application efficiently identifies all repositories located within the specified directories, offering a
comprehensive overview of your projects. GIT List also appends the git path to the '.gitconfig' file.

### How to use GIT List

Run first time?

> [!WARNING]
>
> The `GIT List` bot will overwrite the `$HOME/.gitconfig` file.
> It is strongly recommended to create a backup before executing the `GIT LIST` operation.

Make the `git_list.sh` script executable in the `bot_git_tool` directory.

```
sudo chmod +x source/git_list.sh
```

Then run

```
./source/git_list.sh
```

The GIT List will prompt you for your password to establish a symbolic link within your `/usr/local/bin` directory.
This process is required only once. Additionally, it will generate all the necessary files within your
`$HOME/.config/bot_git_tool/git_list` directory.

Please open the `$HOME/.config/bot_git_tool/git_list/root_directory.conf` file and add the list of root directories
you wish to scan for GIT repositories. add one directory path on each line.

> [!IMPORTANT]
>
> Please avoid adding directories that are high up in the directory tree, such as `/mnt/` or `/`.
> This can slow down the scanning process.

Please open the `$HOME/.config/bot_git_tool/git_list/git_config.conf` file and include all your global Git
configurations. This step is necessary because `GIT List` overrides your default `.gitconfig` file in the home
directory.

To run `GIT List` on any location within your system, open the terminal,

```
gitlist
```

<br>
<br>

# 🫅 Support This Project

Creating and maintaining this project is a labor of love, but it also requires significant time and effort.
Your financial contribution ensures this project remains active, supported, and continues to evolve.

Become a backer and help secure the future of this project:

### [🏆 Donate 🏆][sponsor]

_Thank you for your incredible support!_

<br>
<br>

[bot_git_tool]: https://github.com/iamprogrammerlk/bot_git_tool
[sponsor]: https://iamprogrammer.lk/sponsor
