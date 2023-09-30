# mastering-git
# History: Exploring the past
    git log --graph --decorate --oneline
    git show <sha1>
    git show <branch>
    git show HEAD
    git show HEAD^
    git show HEAD^^
    git show HEAD~2
    git show HEAD~2^2
    git show HEAD@{"1 month ago"}
    git blame <file>
    git diff HEAD HEAD~2
    git diff <branch1> <branch2>
    git log --patch
    git log --grep apples --oneline
    git log -Gapples --patch
    git log -3 --oneline
    git log HEAD~5..HEAD^ --oneline
    git log <branch>..master --oneline

# History: Fixing mistakes
    git commit --amend
    git rebase -i origin/master
        pick <sha1> <log>
        pick <sha1> <log>
        reword <sha1> <edit log>
        squash <sha1> <log>
        squash <sha1> <log>
        pick <sha1> <log>

    git reflog HEAD
    git show HEAD@{15}
    git reflog refs/heads/master
    
    git revert <sha1>
