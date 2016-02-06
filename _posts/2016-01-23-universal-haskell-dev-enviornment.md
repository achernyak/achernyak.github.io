---
layout: post
subtitle: Using Stack and Atom
published: false
title: Universal Haskell development environment
---

## Motivation
Haskell is notoriously difficult to setup, and probably led to many people being scared away from every touching it. However, there has been a lot of work done to address it's short comings. And there is a way to setup a very pleasant environment thanks to the hard work of many projects.

Traditional methods included:
* Installing [The Haskell Platform](https://www.haskell.org/platform/), which was a great project in it's time but always seems to lag a few GHC versions behind.
* Required using a text editor like [Vim](http://www.vim.org/) or [Emacs](https://www.gnu.org/software/emacs/). These are incredible tools and productivity boosters, if you take the time to learn them, but are not for the faint of heart. *I do suggest you learn one of these eventually, or use the vim/emacs mode of another tool.*
* Complex package management through [Cabal-Install](https://wiki.haskell.org/Cabal-Install). This tool caused either version hell from everything being installed globally or caused you to have to re-install all your dependencies for every project.

## Tools of the trade
We will be using these tools to solve the above problems and make the installation completely system agnostic. That's right, this installation process with work on any platform OS X, Linux, and even Windows.
1. [Stack](http://docs.haskellstack.org/) is probably the single biggest win for Haskell in the last year. It makes everything from freshly installing Haskell to creating and building new projects a no brainer.
2. [Atom](https://atom.io/) has become one of my favorite text editors and has great support for Haskell.
3. Item


