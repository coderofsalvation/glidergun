# glidergun

[![CircleCI](https://img.shields.io/circleci/project/gliderlabs/glidergun/release.svg)](https://circleci.com/gh/gliderlabs/glidergun)
[![IRC Channel](https://img.shields.io/badge/irc-%23gliderlabs-blue.svg)](https://kiwiirc.com/client/irc.freenode.net/#gliderlabs)

glidergun allows writing write-once-run-anywhere cli tools using  [Go](https://golang.org) and [Bash](http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO.html).

# Install

    $ curl https://dl.gliderlabs.com/gh/glidergun/latest/$(uname -sm|tr \  _).tgz \
      | tar -zxC /usr/local/bin


# How it works 

The `gun`-command will act as a central point for accessing subcommands written in GO+Bash.
Each subcommand typically consists of:

    mytool/Gunfile             # specify environment variables here
    mytool/cmds                # folder with scripts
   
Check [here](https://github.com/lalyos/gun-github) for an example glidergun application.

# Features:

* intermixing of Go & Bash language using [go-basher](https://github.com/progrium/go-basher). 
* dependency management (`deps-require jq 1.4` e.g.)
* module system
* support for exposing bash functions as subcommands
* easy way to extend tool with subcommands and autocompletion

## Upgrading

	$ gun :update

<img src="https://ga-beacon.appspot.com/UA-58928488-2/glidergun/readme?pixel" />
