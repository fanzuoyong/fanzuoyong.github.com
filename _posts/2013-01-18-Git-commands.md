---
layout: post
title: Git commands
---

# {{ page.title }}

    Press enter to submit commands
    $ git init
    Initialized empty Git repository in /.git/
    Success!
    $ git status
    # On branch master
    #
    # Initial commit
    #
    nothing to commit (create/copy files and use "git -add" to track)
    Success!
    $ git status
    # On branch master
    #
    # Initial commit
    #
    # Untracked files:
    #   (use "-git add <file>..." to- include i-n what wil-l be commi-tted)
    #
    # octocat.txt
    nothing ad-ded to com-mit but un-tracked fi-les presen-t (use "gi-t add" to -track)
    Success!
    $ git add octoc-at.txt
    Nice job, -you've add-ed octocat-.txt to th-e Staging -Area
    $ git statu-s
    # On branch master
    #
    # Initial commit
    #
    # Changes to be committed:
    #   (use "git rm --cached <file>..." to unstage)
    #
    # new file:   octocat.txt
    #
    Success!
    $ git commi-t -m "Add cute octoc-at story-"
    Unmatched -double quo-te: "git c-ommit -m \-"Add cute -octocat st-ory\"\""
    $ git commi-t -m "Add cute octoc-at story-"
    [master (r-oot-commit-) d4c8f51]- Add cute -octocat st-ory
     1 file changed, 1 insertion(+)
     create mode 100644 octocat.txt
    Success!
    $ git add '*.tx-t'
    Unmatched double quote: "git add '*.txt''"
    Did not add "red_octocat.txt"
    $ git add '*.tx-t'
    Success!
    $ git commi-t -m 'Add all the octoc-at txt files-'
    [master 49ee22f] Add all the octocat txt files
     4 files changed, 4 insertions(+)
     create mode 100644 blue_octocat.txt
     create mode 100644 octofamily/baby_octocat.txt
     create mode 100644 octofamily/momma_octocat.txt
     create mode 100644 red_octocat.txt
    Success!
    $ git log
    commit 3f5184a9420f95160b8c68f0daf0b3ebf627a529
    Author: Try Git <try_git@github.com>
    Date:   Fri Jan 18 08:09:33 2013 +0000
    
        Add all the octocat txt files
    
    commit ef43a242048fe5efbbbacc2dc9573f11dfebdad9
    Author: Try Git <try_git@github.com>
    Date:   Fri Jan 18 08:09:33 2013 +0000
    
        Added cute octocat story
    Success!
    >  
    
    
     TryGit—1143x300
    Press enter to submit commands
    $ git remot-e add origi-n git@g-ithub.com:-fanzuoyong-/try_git.g-it
    Success!
    $ git push -u origi-n maste-r
    Branch mas-ter set up- to track -remote bra-nch master- from orig-in.
    Success!
    $ git pull origi-n maste-r
    Merge made by the 'recursive' strategy.
    Success!
    $ git diff HEAD
    diff --git a/octocat.txt b/octocat.txt
    index 7d8d808..e725ef6 100644
    --- a/octocat.txt
    +++ b/octocat.txt
    @@ -1 +1 @@
    -A Tale of Two Octocats
    +A Tale of Two Octocats and an Octodog
    Success!
    $ git add octof-amily/octo-dog.txt
    Success!
    $ git diff --sta-ged
    diff --git a/octofamily/octodog.txt b/octofamily/octodog.txt
    new file mode 100644
    index 0000000..cfbc74a
    --- /dev/null
    +++ b/octofamily/octodog.txt
    @@ -0,0 +1 @@
    +woof
    Success!
    $ git reset- octof-amily/octo-dog.txt
    Success!
    $ git check-out -- octoc-at.txt
    Success!
    $ git branc-h clean-_up
    Success!
    $ git statu-s
    # On branch master
    nothing to commit (working directory clean)
    Use 'git c-heckout' t-o switch t-o the 'cle-an_up' bra-nch
    $ git check-out clean-_up
    Switched to branch 'clean_up'
    Success!
    $ git rm '*.tx-t'
    rm 'blue_octocat.txt'
    rm 'octocat.txt'
    rm 'octofamily/baby_octocat.txt'
    rm 'octofamily/momma_octocat.txt'
    rm 'red_octocat.txt'
    Success!
    $ git commi-t -m "Remo-ve all the cats"-
    [clean_up 70d304d] Remove all the cats
     5 files changed, 5 deletions(-)
     delete mode 100644 blue_octocat.txt
     delete mode 100644 octocat.txt
     delete mode 100644 octofamily/baby_octocat.txt
     delete mode 100644 octofamily/momma_octocat.txt
     delete mode 100644 red_octocat.txt
    Success!
    $ git check-out maste-r
    Switched to branch 'master'
    Success!
    $ git merge- clean-_up
    Updating f5d91ed..1c0864c
    Fast-forward
     blue_octocat.txt             | 1 -
     octocat.txt                  | 1 -
     octofamily/baby_octocat.txt  | 1 -
     octofamily/momma_octocat.txt | 1 -
     red_octocat.txt              | 1 -
     5 files changed, 5 deletions(-)
     delete mode 100644 blue_octocat.txt
     delete mode 100644 octocat.txt
     delete mode 100644 octofamily/baby_octocat.txt
     delete mode 100644 octofamily/momma_octocat.txt
     delete mode 100644 red_octocat.txt
    Success!
    $ git branch -d clean_up
    Deleted branch clean_up (was 0e0527e).
    Success!
    $ git push
    To git@github.com:fanzuoyong/try_git.git
     + fce99d8-...7c210b3- master -> master- (forced u-pdate)
    Success!
    >  
    
