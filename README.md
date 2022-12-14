# Git basics

## Requirements

Before you will use this repository make sure that you have installed:

- ***Git***

  - If you are a **Windows** or **macOS** user visit this link **[Downloading Git](https://git-scm.com/download)**
    then download appropriate installer and install it.
  - If you are a **Linux** (Arch-based distribution) user you can paste bellow scrip into your terminal or visit this
    page **[Installing Git](https://git-scm.com/download/linux)**

    ```bash
    sudo pacman -S git
    ```

- ***GitHub***

  - Create a free account on GitHub. You can find registration form under this
    link **[Create GitHub account](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home)**

If you followed every step, you should be ready to start using this repository. To make sure that you have installed
everything correctly open your terminal git-bash and run the following commands:

- To check **git**: `git --version` → you should see output with git version

## Downloading the repository

- Open your terminal / git-bash in location where you create a directory which will contain this repository
- Run the following command in your terminal / git-bash

  ```bash
  git clone https://github.com/GDSC-Lodz-University-of-Technology/git-basics.git
  cd ./git-basics
  ```

## Workshops aim

At the end of this workshop, you should have a basic understanding git.
You should also know the most important features of GitHub platform.

## Resources

- Learn how to use GitHub with interactive courses designed for beginners and
  experts ***[GitHub Skills](https://skills.github.com/)***
- Learn Git by playing computer game ***[Learn Git Branching](https://learngitbranching.js.org/)***
- Video Git tutorial in
  polish ***[Kurs Git po polsku od podstaw](https://www.youtube.com/watch?v=D6EI7EbEN4Q&list=PLjHmWifVUNMKIGHmaGPVqSD-L6i1Zw-MH&index=1)***
- Git documentation ***[Gid Documentation](https://git-scm.com/doc)***
- Set of rules how to write good commit
  messages ***[Conventional commit](https://www.conventionalcommits.org/en/v1.0.0-beta.4/)***
- Markdown syntax, used to create documentation ***[Basic Syntax](https://www.markdownguide.org/basic-syntax/)***

## Git tree alias

If you would like to use same formatting for logging git tree in terminal you can use this configuration:

```bash
git log --graph --pretty=format:'%Cred%H%Creset %C(yellow)%d%Creset %n %s %n %C(bold blue)<%an>%Creset %Cgreen(%cs, %cr)' --abbrev-commit --date=relative --branches
```

You can also save this command under *[alias](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)* to make easier to
use in the future

```bash
git config --global alias.tree "log --graph --pretty=format:'%Cred%H%Creset %C(yellow)%d%Creset %n %s %n %C(bold blue)<%an>%Creset %Cgreen(%cs, %cr)' --abbrev-commit --date=relative --branches"
```

> Now you can run `git tree` to see the results
