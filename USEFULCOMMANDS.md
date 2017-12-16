# Useful Commands
## Send stdout to both console and a file
foo | tee output.file
create-react-app sandbox-reason --scripts-version reason-scripts | tee ../../COMMANDS-and-LOGS/react/create-react-app_sandbox-reason_2017_11_23


## Git (and Github)
* SSH
	* [Github Guide](https://help.github.com/articles/checking-for-existing-ssh-keys/)
* Show branches
	* `git branch`
	* (To see last commit on each bracnh) `git branch -v`
	* (Just show merged branches) `git branch --merged`
	* (Just show unmerged branches) `git branch --no-merged`
	* [More Info](https://git-scm.com/book/en/v2/Git-Branching-Branch-Management)

* Show branches on the remote origin repo (e.g. Github)
	* `git remote show origin`

* Show branches on the remote upstream - the repo that origin was forked FROM
	* `git remote show upstream`

* Show all branches, both local and remote
	* `git branch -a`
	* [More info on remote branches](http://gitready.com/intermediate/2009/02/13/list-remote-branches.html)

* Show commit history
	* `git log`
	* [More Info on viewing commit history](https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History)

* (Hard) reset to previous commit
	* `git reset --hard <commithash>`

* Add upstream repository
	* `git remote add upstream git@github.com:sketch-city/harvey-api.git`

* Show upstream
	* `git remote show upstream`

* Get a new branch from the upstream repository
	* `git checkout -t upstream/<new branch>`

* Push that new branch to your/origin/forked repository
	* `git push origin <that new branch>`





## PostgreSQL
* Start the server
	* `pg_ctl -D /usr/local/var/postgres -l logfile start`
	or
	* `brew services start postgresql`

* Create a new user with a password
	* `createuser <username> -P`

* start psql with a specific user
	* `psql -U <username`

* quit psql
	* `\q`


## Rails



## Unix
### ln command

Example: ```ln /CS_Book/USEFULCOMMANDS.md /COMMANDS-and-LOGS/USEFULCOMMANDS.md```
