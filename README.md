# .gitconfig

[filter "lfs"]
	clean = git-lfs clean -- %f
	smudge = git-lfs smudge -- %f
	process = git-lfs filter-process
	required = true
[user]
	email = cawauchi6204@gmail.com
	name = cawauchi6204
[difftool "sourcetree"]
	cmd = opendiff \"$LOCAL\" \"$REMOTE\"
	path = 
[mergetool "sourcetree"]
	cmd = /Volumes/outerSSD/Sourcetree.app/Contents/Resources/opendiff-w.sh \"$LOCAL\" \"$REMOTE\" -ancestor \"$BASE\" -merge \"$MERGED\"
	trustExitCode = true
[alias]
	s = status
	br = branch
	brm = branch -m
	brd = branch -d
	brdd = branch -D
	co = checkout
	cob = checkout -b
	adu = add -u
	adup = add -u -p
	cm = commit
	mg = merge --no-ff
	mgff = merge --ff
	cp = cherry-pick
	log1 = log -1
	log2 = log -2
	log3 = log -3
	logo = log --oneline
	logn = log --name-status --oneline
	firstcom = commit --allow-empty -m \"Initial commit\"
	df = diff
