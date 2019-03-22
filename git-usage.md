# Git learning

## config
	git config --global core.editor vim
	git config --list

## help dispaly
	detail messages: git --help log or show or commit

	brief messages: git log/show/commit -h

## combine root commit
	git rebase -i --root

## hide the changes
	git stash
	git stash pop

## the test branch merge to master
	git checkout master
	git merge test

## submodule
	(1) parent directory run command, generate .gitmodules
	git submodule add https://github.com/XzxEmbedded/atomthreads.git
	(2) next clone repo, parent directory run command
	git submodule update --init --recursive

## delete remote branch
	git push origin --delete branch-name

## format-patch
	git format-patch -1

## git tag
	git tag tag-names

	note: git tag can't pull request

## git log --grep
	git log --grep "find strings"

## git revert
	notes: revert before commit
	git revert commit-id

## Merge pull request for deleting merge commit name
	Commandline merge, Step2:
	git merge --no-commit branch_merge

## cherry-pick
	merge anther branch commit id to current branch
	git cherry-pick commit-id

## git add -u
	Add modify files into working area again

## git reset HEAD
	Recover working area

## git remote add remote-repo-name https://xzx.git(remote-repo-address)
	Add new remote repo

## git checkout
	git checkout file-name, it will back to modifying file.
	git checkout branch-name, it will change branch.

## git clean
	Clean not staged files.
	-n: try running
	-f: delete file
	-d: delete directory
