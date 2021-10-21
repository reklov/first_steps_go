My steps to setup my Mac with OSX to get productive. Writing docs withto programm with go and Google Cloud plattform

Tested on: OSX Big Sour



# First steps to _GO_ productive

## Textmate - Text editor

Powerful and customizable text editor with support for a huge list of programming languages and developed as open source.

Visit: https://macromates.com/

One important part after the installation is to enable the _Shell Support_

Inside textmate Go to _Preferences_ -> _Terminal_ -> Choose _Install Shell Support_

## iTerm2 - Terminal App

iTerm2 is a replacement for Terminal and the successor to iTerm. It works on Macs with macOS 10.14 or newer. iTerm2 brings the terminal into the modern age with features you never knew you always wanted.

Visit: https://iterm2.com/

## Homebrew - Package Manager

The Missing Package Manager for macOS (or Linux)

https://brew.sh/

## ssh key

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

// Adding SSH Key
// Azure DevOps
// Github

## Special Fonts

we use some special fonts, that make Code much more readable.

Visit:  https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k
Visit:  https://www.jetbrains.com/lp/mono/

Do not forget to use this fonts in your coding editor and in iterm

## Powerlevel10k - Terminal Enanchment

```bash
brew install brew install romkatv/powerlevel10k/powerlevel10k
```

Adding this to your zsh config

`echo "source $(brew --prefix)/opt/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc`

Starting the configuration

```bash
source /usr/local/opt/powerlevel10k/powerlevel10k.zsh-theme
```

Reconfigure your p10k installation

`p10k configure`

Visit: https://github.com/romkatv/powerlevel10k for more information

## Programming languages

### Golang

`brew install go`

simple test for your go installation:

`go version`

Visit: https://golang.org/doc/tutorial/getting-started for a more detailed test.

## VS Code // Golang Jetbrains

Choose one or both

Visit: https://code.visualstudio.com/

Visit: https://www.jetbrains.com/go/

## Typora - Markdown Text editor

Minimal Markdown Editor

Visit: https://typora.io/

## hugo - Static site generator

The world’s fastest framework for building websites

https://gohugo.io/

`brew install hugo`

 https://gohugo.io/getting-started/installing

## Chrome extension

Some useful extensions

- JSON Formatter

## Google SDK

https://cloud.google.com/sdk

test your installation:

`gcloud auth login`
