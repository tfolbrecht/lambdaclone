# README

## I wrote this because sometimes I would:

* forget to fork, and would work against the master repo.
* forget to start a branch, and would accidentally work on the master branch
* forget to set my upstream origin, and would have to stop my flow and fix that
* Forget to add my project manager, and they miss out on notifications on my commits
* Run git clone in the wrong directory, and have to delete it, and reclone 

Now I just run `lambdaclone`

## Getting started

You must fill out the scripts variables with the following


| Bash Variables | Values |
| ----- | :-----|
| user                  | Your GitHub Username |
| secretkey             | Your [GitHub Token](https://github.com/settings/tokens)|
| branch_name           | The name of the branch you create, I use firstname-lastname |
| PMuser                | Your PM's Username |
| project_parent_path   | The path to the directory you wnat to clone to |

*note,* *not the most secure method of storing api keys lol*

Move script somewhere in your user execution path like `/usr/local/bin/` or `~/.local/bin`

## Todo

- ~~Check if variables empty~~
- test against multiple configurations
- check credential validity
- support non ssh
- make github api only version (fork, add collaborator, set branch)
- best practice api key storage
- auto open editor with new repo path
- interactive ncurses menu, options, etc