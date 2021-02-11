## `git`

### Commands

- [Undoing Changes in Git](https://pbs.twimg.com/media/B6G1QPnCEAANZCF.png)
- [`git-worktree`](https://git-scm.com/docs/git-worktree) - Manage multiple worktrees attached to teh same repository

### Converting a Mercurial (`hg`) Repository to `git`

```sh
cd ~
git clone git://repo.or.cz/fast-export.git
git init new_git_repo
cd new_git_repo
~/fast-export/hg-fast-export.sh -r /path/to/old/mercurial_repo
git checkout HEAD
git repack -a -d --depth=250 --window=250
```

(Thanks to [akluth](http://stackoverflow.com/users/1616951/akluth)'s answer on [Convert Mercurial project to Git](http://stackoverflow.com/questions/16037787/convert-mercurial-project-to-git)) and Linus Torvalds' mail quoted in [this post](https://metalinguist.wordpress.com/2007/12/06/the-woes-of-git-gc-aggressive-and-how-git-deltas-work/) for this solution).


### Controlling SSH key file

- [Select Private key to use with `git`](https://stackoverflow.com/questions/6688655/select-private-key-to-use-with-git)
- [Specify an SSJ key for git push for a given domain](https://stackoverflow.com/questions/7927750/specify-an-ssh-key-for-git-push-for-a-given-domain)
