# Git Basic Commands

## Install VSCode and Set Up 'code' Command in Terminal
I think VSCode is one of the main tools one have to have installed while trying to work with Git. VSCode comes with git if you are using Mac, if using Windows install git and gitbash.

- Open Visual Studio Code
- Open the Command Palette by pressing **cmd + shift + P**
- Install 'code' command in PATH by typing **Shell Command: Install 'code' command in PATH**
- Select the option and press Enter
- Restart the terminal

## Let's create our working folder
Let's create a folder and in order to be able initialize git

Create a folder
```shell
$ mkdir git-project
$ cd git-project
```

Open a new instance of Visual Studio Code
```shell
$ code ./
```

## Initial Git Configuration
Let's add our information to track our authoring

```shell
$ git config --global user.name "username"
$ git config --global user.email mymail@mail.com
```

## Let's Initialize Git
We can initialize a new repository just by being local.

```shell
$ git init
```
