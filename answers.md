git version 2.17.1

user.name=Brian Hartman
user.email=bh018420@ohio.edu

NAME
       git-add - Add file contents to the index

SYNOPSIS
       git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p]
                 [--edit | -e] [--[no-]all | --[no-]ignore-removal | [--update | -u]]
                 [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormali
ze]
                 [--chmod=(+|-)x] [--] [<pathspec>...]

DESCRIPTION
       This command updates the index using the current content found in the working tree, to
       prepare the content staged for the next commit. It typically adds the current content of
       existing paths as a whole, but with some options it can also be used to add content with
       only part of the changes made to the working tree files applied, or remove paths that do
       not exist in the working tree anymore.

       The "index" holds a snapshot of the content of the working tree, and it is this snapshot
       that is taken as the contents of the next commit. Thus after making any changes to the
       working tree, and before running the commit command, you must use the add command to add
       any new or modified files to the index.

       This command can be performed multiple times before a commit. It only adds the content of
       the specified file(s) at the time the add command is run; if you want subsequent changes
       included in the next commit, then you must run git add again to add the new content to the
       index.

       The git status command can be used to obtain a summary of which files have changes that are
       staged for the next commit.

       The git add command will not add ignored files by default. If any ignored files were
       explicitly specified on the command line, git add will fail with a list of ignored files.
       Ignored files reached by directory recursion or filename globbing performed by Git (quote
       your globs before the shell) will be silently ignored. The git add command can be used to
       add ignored files with the -f (force) option.

       Please see git-commit(1) for alternative ways to add content to a commit.

On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.md
        answers.md

nothing added to commit but untracked files present (use "git add" to track

On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   README.md
        new file:   answers.md

[master (root-commit) 8174464] Initial commit
 2 files changed, 70 insertions(+)
 create mode 100644 README.md
 create mode 100644 answers.md

commit 8174464638a6cc905a5129dc3f552a86c5d2388c (HEAD -> master)
Author: Brian Hartman <bh018420@ohio.edu>
Date:   Wed Jan 25 18:45:20 2023 -0500

    Initial commit

Counting objects: 4, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 1.35 KiB | 1.35 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/Bhartman4/git-lab.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.

Brian Hartman
Bhartman4

Brian Hartman
Bhartman4
CS 2400
Section 107

Already up to date.
Brian Hartman
Bhartman4
CS 2400
Section 107

.  ..  git-lab-2  Labs