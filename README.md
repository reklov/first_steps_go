# First steps to _GO_ productive

My steps to setup my Mac with OSX to get productive. Writing docs to programm with Golang and Google Cloud plattform. Programming with Windows 10 is certainly also possible and I tried a lot of stuff and used Windows 10 with ther terminal app and WSL2. But for short: OSX is much more comfortable and faster. So if you have the possiblity to use osx, then do it.

I noted here all steps I do to setup a plain OSX as my developer environment.

Tested on mac OS: ==Big Sour== ==Monterey==

# Homebrew - Package Manager

First we will need to install [Homebrew](https://brew.sh/). Homebrew is the Missing Package Manager for macOS (or Linux), that installs the packages that Apple didn´t. We will use brew to install some stuff with much less effort compared to doing everything manually.

Open your ==Terminal== and copy the text below:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Visit https://brew.sh/ to learn more about it!

## Update Homebrew

After you installed Homebrew you can and certainly should open your ==Terminal==  and update brew from time to time with 

```bash
brew update
```

after running that command it shows you all outdated installed packages.
to update all and everything just type

```bash
brew upgrade
```

# iTerm2 - Terminal App

Using the terminal is one of the biggest productivity boosts you can gain in your daily work as a developer. You will be way faster than using the UI and the mouse.
But there is one problem, the standard ==Terminal.app==  provided by Apple is quite basic. So we will replace it with [iTerm2](https://iterm2.com/) to have a modern, feature blown terminal on our hands. After installing iTerm2, everytime when I talk about terminal in this script about I always mean iTerm2 or in short iTerm.
Installing iTerm2 ist easy, we simply use.

Open your ==Terminal== and copy the text below:

```bash
brew install --cask iterm2
```

Visit: https://iterm2.com/ to learn more about it!

# Powerlevel10k - Terminal Enanchment

Powerlevel10k is a theme for Zsh. It give you all neccessarz infomation, that you will need while working with the terminal. So it will save you time. In example it informs you on the current git state or the branch you are working on. 

Visit: https://github.com/romkatv/powerlevel10k for more information

## Install

Copy this comands to you ==Terminal== (And now we are using ==iTerm==)

```bash
brew install romkatv/powerlevel10k/powerlevel10k
echo "source $(brew --prefix)/opt/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
source ~/.zshrc
```

##Reconfigure p10k

While you are configuring powerlevel10k you will asked a lot of questions. And it is very likely, that you want to change some of your settings later. 
To do so just type this command on your ==Terminal== 

```bash
p10k configure
```

# VS Code

[Visual Studio Code]( https://code.visualstudio.com/) from Microsoft is a very resource-efficient editor. It is a good starting point and help you also to edit resource files. If you later do some more heavy development stuff I highly recommend to have a look at the tools from [Jetbrains](https://www.jetbrains.com)

Visit: https://code.visualstudio.com/ for more information

To install Visual Studio Code we simply can use brew. Just type this into yout terminal.

```
 brew install --cask visual-studio-code
```

## Launching from the command line

Working at the terminal make s you much faster. But often you simply want to edit a file, without then using the UI and navigate to the folder, where you already are at the terminal. What could be better, than starting the editor right from the place, whre you are at the terminal. To do so you need to follow these steps: https://code.visualstudio.com/docs/setup/mac

After this you are able to open Visual Studio Code right from the terminal like this.

```
code .
```

This will open the entire directory inside your editor.

```
code some.txt
```

will open the file _some.txt_ in your editor.

# Programming languages

## Golang

```bash
brew install go
```

simple test for your go installation:

```bash
go version
```

where to put your go files?

Visit: https://golang.org/doc/tutorial/getting-started for a more detailed test and a good starting point with the golang language.


# Markdown

> **Markdown** is a [lightweight markup language](https://en.wikipedia.org/wiki/Lightweight_markup_language) for creating [formatted text](https://en.wikipedia.org/wiki/Formatted_text) using a [plain-text editor](https://en.wikipedia.org/wiki/Text_editor). [John Gruber](https://en.wikipedia.org/wiki/John_Gruber) and [Aaron Swartz](https://en.wikipedia.org/wiki/Aaron_Swartz) created Markdown in 2004 as a [markup language](https://en.wikipedia.org/wiki/Markup_language) that is appealing to human readers in its source code form.[[9\]](https://en.wikipedia.org/wiki/Markdown#cite_note-philosophy-9) Markdown is widely used in [blogging](https://en.wikipedia.org/wiki/Blog), [instant messaging](https://en.wikipedia.org/wiki/Instant_messaging), [online forums](https://en.wikipedia.org/wiki/Online_forums), [collaborative software](https://en.wikipedia.org/wiki/Collaborative_software), [documentation](https://en.wikipedia.org/wiki/Documentation) pages, and [readme files](https://en.wikipedia.org/wiki/README).

from [Wikipedia](https://en.wikipedia.org/wiki/Markdown)

Using a markup language instead of MS Word or others has the clear benefit, that you can use a version control system like ==Git==

## Typora - Markdown Text editor

Also Visual Studio code has some cabapilities to edit and preview Markdown files. There is a better alternative. It is not for free, but worth the money. 

Visit: https://typora.io/

## hugo - Static site generator

The world’s fastest framework for building websites.

https://gohugo.io/

`brew install hugo`

 https://gohugo.io/getting-started/installing

# Google SDK

To develop with the Google Cloud Plattform (GCP) you will need the GCP SDK. 

Visit: https://cloud.google.com/sdk/docs/install to download the necessary files.


