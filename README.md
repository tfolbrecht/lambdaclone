# I wrote this because sometimes I would:

* forget to fork, and would work against the master repo.
* forget to start a branch, and would accidentally work on the master branch
* forget to set my upstream origin, and would have to stop my flow and fix that
* Forget to add my project manager, and they miss out on notifications on my commits
* Run git clone in the wrong directory, and have to delete it, and reclone 

Now I just run `lambdaclone git@github.com:tfolbrecht/lambdaclone.git`

## Getting started

You must fill out the scripts variables inside quotes " with the following


| Bash Variables | Values |
| ----- | :-----|
| user                  | Your GitHub Username |
| secretkey             | Your [GitHub Token](https://github.com/settings/tokens)|
| branch_name           | The name of the branch you create, I use firstname-lastname |
| TLuser                | Your TL's Username |
| project_parent_path   | The path to the directory you wnat to clone to |
| subdir_weeks          | Set to true if you want to use Week_## subdirectory structure |
| editor_bin            | Specify editor command |
| debug                 | Set to true to output debugging messages |

*note,* *not the most secure method of storing api keys lol*

Move script somewhere in your user execution path like `/usr/local/bin/` or `~/.local/bin`

## Todo

- ~~Check if variables empty~~
- ~~auto open editor with new repo path~~
- test against multiple configurations
- check credential validity
- support non ssh
- make github api only version (fork, add collaborator, set branch)
- best practice api key storage
- interactive ncurses menu, options, etc
