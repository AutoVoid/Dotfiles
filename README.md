dotfiles
========
If you're curious how to setup your own dotfiles, please visit [Mathias Bynens's dotfiles](https://github.com/mathiasbynens/dotfiles) to learn more.

## Sync

The guide on how to keep your dotfiles in sync.

If've haven't yet clones this repository, fire up your terminal and clone this repository to your environment.

```bash
git clone git@github.com:vinkla/dotfiles.git
```

Whenever there are new updates, try to stay in sync and pull them down.

```bash
git pull
```

Then execute the bootstrap shell script to get the latest changes.

```bash
source bootstrap.sh
```

## Installation

This is the installation guide to setup these dotfiles on a new OS X system.

Install XCode Command Line Tools.

```bash
xcode-select --install
```

Install Homebrew [http://brew.sh](http://brew.sh).

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Install GIT [http://git-scm.com](http://git-scm.com).

```bash
brew install git
```

Generate SSH keys [https://help.github.com/articles/generating-ssh-keys](https://help.github.com/articles/generating-ssh-keys)

```bash
ssh-keygen -t rsa -C "your_email@example.com"
```

Clone this respoitory and install dotfiles.

```bash
git clone git@github.com:vinkla/dotfiles.git
source bootstrap.sh
```

Install binaries and native Mac applications.

```bash
source ./scripts/brew && source ./scripts/cask
```

Create Sites directory in home root folder.

```bash
mkdir ~/Sites
```

Run the OSX setup script.

```bash
source ./scripts/osx
```

Restart the computer and live happily ever after.

## License

The dotfiles repository is licensed under [The MIT License (MIT)](LICENSE).

