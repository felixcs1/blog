# WIP blog

Setup: 
- https://gohugo.io/hosting-and-deployment/hosting-on-github/
- https://themes.gohugo.io/hugo-theme-hello-friend/
- 

Commands to add theme and delpoy repo
- `git submodule add https://github.com/panr/hugo-theme-hello-friend.git themes/hello-friend`
- `git submodule add -b main git@github.com:felixcs1/felixcs1.github.io.git public`

Deploy
- `./deploy.sh "commit message"`


Remove a submodule
- Delete the relevant section from the .gitmodules file.
- Stage the .gitmodules changes git add .gitmodules
- Delete the relevant section from .git/config.
- Run git rm --cached path_to_submodule (no trailing slash).
- Run rm -rf .git/modules/path_to_submodule (no trailing slash).
- Commit git commit -m "Removed submodule "
- Delete the now untracked submodule files rm -rf path_to_submodule