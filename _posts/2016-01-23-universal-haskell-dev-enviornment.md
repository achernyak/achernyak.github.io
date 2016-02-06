---
layout: post
subtitle: Using Stack and Atom
published: false
title: Universal Haskell development environment
---

## Motivation
Haskell is notoriously difficult to setup, which probably led to many people being scared away from ever getting started. However, there has been a lot of work done to address these short comings. And there is a way to setup a very pleasant environment thanks to the hard work of many projects.

Traditional methods included:
* Installing [The Haskell Platform](https://www.haskell.org/platform/), which was a great project in it's time but always seems to lag a few GHC versions behind.
* Required using a text editor like [Vim](http://www.vim.org/) or [Emacs](https://www.gnu.org/software/emacs/). These are incredible tools and productivity boosters, if you take the time to learn them. Which is a pretty major time commitment in itself *I do suggest you learn one of these eventually, or use the vim/emacs mode of another tool.*
* Complex package management through [Cabal-Install](https://wiki.haskell.org/Cabal-Install). This tool caused either version hell from everything being installed globally or caused you to have to re-install all your dependencies for every project.

## Tools of the trade
We will be using these tools to solve the above problems and make the installation completely system agnostic. That's right, this installation process with work on any platform OS X, Linux, and even Windows.
1. [Stack](http://docs.haskellstack.org/) is probably the single biggest win for Haskell in the last year. It makes everything from freshly installing Haskell to creating and building new projects a no brainer.
2. [Atom](https://atom.io/) has become one of my favorite text editors and has great support for Haskell.
That's it those are the two major tools you will need to install and everything else is done through packages for them. Go ahead and install these from their respective websites.
## The setup
Now let's crack open the terminal and configure our environment. All the commands will remain the same regardless of your operating system. 

The easiest part to install is the atom packages. It's just one line.
    $ apm install language-haskell haskell-ghc-mod ide-haskell-cabal ide-haskell autocomplete-haskell
Next we need to install Haskell, or GHC to be more specific. Stack does not come GHC but it does come with an easy way to install it.
    $ stack setup
Now, for all the atom packages to work. We will need a few Haskell packages installed. These are all very simple to install except `ghc-mod` has a quirk with it's dependencies.

