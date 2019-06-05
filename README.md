# repeater

repeater is a simple utility which can be used to quickly scaffold a directory structure

it works off a pre-defined template which exists as a github repo

e.g.,

rptr init robspassky/rptr-java-spring .

will use http://github.com/robspassky/rptr-java-spring.git as a template to populate the current
directory (or another specified child directory, if the child does not exist, it will be created)

it works like this:

1. clone the github repo to a local tmp directory
2. run .rptr/initial.sh
3. prompt for updating default variables (.rptr/vars)
4. copy files/directories from repo to target directory
5. run .rptr/final.sh

