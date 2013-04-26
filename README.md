# Jenkins Command Line Interface

> **Interact with Jenkins from you terminal.** Launch build process, watch logs or search projects without your mouse!

## Usage

    $ jenkins build My-Awesome-Project

Build the project on Jenkins, and displays the result when the operation is complete.
Use `-v` for verbose mode

    $ jenkins list

List all available projects

    $ jenkins log My-Awesome-Project

Display logs of last build(ed) project

    $ jenkins list *capdemat* 

**TODO** Search over projects

    $ jenkins checkout My-Awesome-Project new-git-branch

**TODO** Alter git branch on the fly

## Prerequisites

Required dependencies

* Perl
* Jsawk (https://github.com/micha/jsawk) `brew install jsawk`

## Installation

Set your Jenkins credentials. The token is accessible in [your account](http://build-01.znx.fr/user/JLA@zenexity.com/configure).

    export JENKINS_LOGIN="xxx@zenexity.com"
    export JENKINS_TOKEN="xxxxxxxxxxxxxxxxxxxxxxxxxxx"

Clone the project

    git clone git@github.com:studiodev/jenkins-cli.git
    chmod +x jenkins-cli/jenkins
    
It's ready! But you could add jenkins-cli to your PATH or create an alias to use it from everywhere.
