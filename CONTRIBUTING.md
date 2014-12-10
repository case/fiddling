# Contributing

1.  Fork the project and clone your fork.

1.5 [Configure a remote for the fork](https://help.github.com/articles/configuring-a-remote-for-a-fork/).

		$ git remote -v
		$ git remote add upstream https://github.com/case/fiddling.git

2.  Create a local feature branch:

        $ git checkout -b <branch>

2.5 [Keep the fork in sync](https://help.github.com/articles/syncing-a-fork/)

		$ git fetch upstream
		$ git checkout master
		$ git merge upstream/master

2.6 Keep your feature branch in sync?

3.  Make one or more atomic commits. Include unit tests if adding a function
    or fixing a bug. Each commit should have a descriptive commit message,
    wrapped at 72 characters.

4.  Run all tests and linters, and address any errors. Preferably, fix
    commits in place using `git rebase` or `git commit --amend` to make the
    changes easier to review and to keep the history tidy.

5.  Push to your fork:

        $ git push origin <branch>

6.  Open a pull request.