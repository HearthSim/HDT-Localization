# HDT-Localization
This is the localization repo for [HearthSim/Hearthstone-Deck-Tracker](https://github.com/HearthSim/Hearthstone-Deck-Tracker)


## How to contribute

### Setup
1. Download and install [git](https://gist.github.com/derhuerst/1b15ff4652a867391f03). 
2. Download and install [ResX Resource Manager](https://resxresourcemanager.codeplex.com/)
3. Fork the repo ("Fork"-button in the top right)
3. Clone the repo:  
  4.1 Open the command prompt (press Win+R, type "cmd" and click Ok)  
  4.2 Navigate to the desired location (e.g. "C:/Github"): `cd "C:/Github"`  
  4.3 Clone the repo `git clone https://github.com/{YOUR_GITHUB_NAME}/HDT-Localization` (this is the url you got redirected to after forking the repo).  
  4.4 Move into the repo directory `cd HDT-Localization`.
  
### Make sure your fork is up to date
(You can skip this if you just completed the setup step)
1. Add the original repo as the upstream source. This only needs to be done once.  
```
git remote add upstream https://github.com/HearthSim/HDT-Localization
```
2. Reset your local copy to upstream (**this will discard any local changes!**)  
```
git fetch upstream
git checkout master
git reset --hard upstream/master
```
3. Reset your fork to upstream  
```
git push origin master --force
```

### Make changes
#### Make changes locally
1. Make sure your fork is up to date (see above)
2. Run ResX Resource Manager
3. Set `C:/Github/HDT-Localization` (or your respective location) as the directory
4. (Optional) To add a new language click the "Add new language" button at the top and select your language. Choose the one containing the country identifier if available - "da-DK" rather than "da".
5. Make the desired changes to your language.
6. Save.

#### Push changes to your fork
1. Stage your changed files `git add {FILE_YOU_MODIFIED}`. Usually this should be just one, you can see all modified files via `git status`.
2. Commit your changes `git commit -m "{YOUR_COMMIT_MESSAGE}"`. Obligatory [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/) - however something like "{LANGUAGE} update {DATE}" (e.g. "Polish update 05.02.2018") is sufficient here.
3. Push to your fork `git push`  
You can do these 3 steps as often as desired in the process to save your work online.

#### Get your changes merged
- [Create a pull request](https://help.github.com/articles/creating-a-pull-request/) and wait for it to get merged. You can push further changes (as described above) while the pull request is open and it will automatically update.


## License

This project is licensed under the CC0 1.0 Universal license (Public Domain).
The full license text is available in the LICENSE file.
