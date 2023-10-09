# git-scripts
A collection of git bash scripts, particularly related to submodule handling.


## Scripts

- git-a-dog: Shortcut to a common spell to display git as a one-line graph.
- git-checkout-and-update [branch]: If a branch name is provided as an argument it will check out that branch, otherwise it gets the current branch's name. Then it will try to check out the same branch name in all submodules, but if that's not possible then `dev`, `main` and `master` are attempted in that order. If any succeeds then a `git pull` is executed, otherwise an error is thrown.
- git-config-user email name: Sets the git user information in this repository an all submodules without touching the global config. Ideal if you don't want to set up a global user config to ensure separation between work and personal projects on the same machine.
