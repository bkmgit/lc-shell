---
title: Setup
---

To participate in this Library Carpentry lesson, you will need a working Unix-like shell environment. We will be using Bash ([Bourne Again Shell](https://en.wikipedia.org/wiki/Bash_\(Unix_shell\))) which is standard on Linux and macOS. Some macOS users (Catalina or later) will have zsh (Z shell) as their default version. Even if you are a Windows or Android user, learning Bash will open up a powerful set of tools on your personal machine, and familiarize you with the standard remote interface used on most servers and supercomputers.

::::::::::::::::::::::::::::::::::::::::::  prereq

## Terminal Setup

Bash is the default shell on most Linux distributions and older versions of macOS. Windows users will need to install Git Bash to provide a Unix-like environment.  Android users will need to install Termux.

- **Linux:** The default shell is usually Bash, but if your machine is set up differently you can run it by opening a terminal and typing `bash` followed by the <kbd>enter</kbd> key. There is no need to install anything. Look for Terminal in your applications to start the Bash shell.

- **macOS:** Open Terminal from `/Applications/Utilities` or Spotlight Search. In versions before Catalina, Bash is the default shell, so you do not need to do anything further. In Catalina and onwards, the default shell is zsh, which is similar but may behave differently from Bash in some cases. To switch to Bash, enter the command `bash` in your terminal window followed by the <kbd>enter</kbd> key.

- **Windows:** On Windows, CMD or PowerShell are normally available as the default shell environments. These use a syntax and set of applications unique to Windows systems and are incompatible with the more widely used Unix utilities. However, a Bash shell can be installed on Windows to provide a Unix-like environment. For this lesson we suggest using Git Bash, part of the >[Git for Windows](https://gitforwindows.org/) package:
  
  - Download the latest Git for Windows [installer](https://gitforwindows.org/).
  - Double click the `.exe` file to run the installer (for example, `Git-2.42.0.2-64-bit.exe`) using the default settings.
  - Once installed, open the shell by selecting Git Bash from the start menu (in the Git folder).

  There are also some more advanced solutions available for running Bash commands on Windows. A Bash shell command-line tool is available for Windows 10, which you can use if you enable the [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10). You can also run Bash commands on a remote computer or server that already has a Unix Shell from your Windows machine. This can be done through a Secure Shell (SSH) client. One client available for free for Windows is [PuTTY](https://www.putty.org/).

- **Android:** On Android [Termux](https://termux.dev/en/) provides a Bash shell environment:
  
  - Either install [F-droid](https://f-droid.org/en/) and then install [Termux](https://f-droid.org/en/packages/com.termux/), or download the [Termux APK file](https://f-droid.org/en/packages/com.termux/) and install it directly.  Be sure to download these from reputable sources, either F-droid or the official GitHub releases.
  - Once installed, start Termux and get the packages needed
```
pkg update && pkg upgrade
pkg install emacs
pkg install nano
pkg install wget
```

::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::  prereq

## Data Files

You need to download some files to follow this lesson:

1. Download [shell-lesson.zip](data/shell-lesson.zip) and move the file to your Desktop.
2. Unzip/extract the file (ask your instructor if you need help with this step). You should end up with a new folder called `shell-lesson` on your Desktop.
3. Open the terminal and type `ls` followed by the <kbd>enter</kbd> key.

    ```bash
    $ ls
    ```

    You should see a list of files and folders in your current directory.

4. Then type:

    ```bash
    $ pwd
    ```

    This command will show you where you are in your file system, which should now be your home directory. In the lesson, you will find out more about the commands `ls`, `pwd` and how to work with the data in `shell-lesson` folder.

::::::::::::::::::::::::::::::::::::::::::::::::::
