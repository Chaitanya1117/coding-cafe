# Lab 4: Git & GitHub — Notes

## Question 1

What did `--global` mean here? What would happen if you left it out? Guess, then check with `man git-config` or ask.

**Answer:** The `--global` option saves the Git configuration for my user account, so it applies to all my repositories by default. If I leave it out, the setting applies only to the current repository.

## Question 2

What appeared in `ls -a` but not in `ls`? What is inside it?

**Answer:** The `.git` directory appeared in `ls -a` but not in `ls` because it is a hidden directory. It stores Git's repository data, including commit history, configuration, and other information needed to track changes.

## Question 3

Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did *not* write?

**Answer:** Git listed the files and folders in my project that were not yet tracked. Some items may be generated files or folders, such as virtual environment files, that I did not write myself.

## Question 4

Compare this `git status` with the one from Question 3. What disappeared?

**Answer:** After adding the `.gitignore` file, Git stopped listing files and folders matching the ignore rules. These include `.venv/`, `__pycache__/`, `*.pyc`, and `.DS_Store`.

## Question 5

`.gitignore` itself shows up as untracked. Should it be committed, or ignored too? Why?

**Answer:** The `.gitignore` file should be committed because it tells Git which files and folders to ignore. Committing it ensures that other people working on the repository use the same ignore rules.

## Question 6

`README.md` moved from one heading to another in the `git status` output. Which two? In the three-places model from the session, what just happened to it?

**Answer:** `README.md` moved from **Untracked files** to **Changes to be committed**. Running `git add README.md` staged the file, moving it into the staging area so it could be included in the next commit.

## Question 7

What did Git print after the commit? How many files did it say changed?

**Answer:** Git displayed a message confirming that the commit was created, along with a summary of the files changed. The exact number of files changed is the number shown in my terminal after running `git commit`.

## Question 8

What are the first seven characters of your commit called, and what are they for?

**Answer:** The first seven characters are the short form of the commit hash. They identify a commit and can be used to refer to it without typing the full hash.

## Question 9

You now have two commits. Without looking it up: what are the four steps of the loop you just did twice?

**Answer:** The four steps are edit, stage, commit, and repeat. Editing changes a file, staging selects changes for the next commit, and committing saves a snapshot in the repository history.

## Question 10

Why does this file get a special name and a special place, rather than being called `notes.md` like everything else?

**Answer:** `README.md` is a standard filename that GitHub recognizes and displays on the repository's front page. It gives visitors an introduction to the project and explains its contents.

## Question 11

What did `gh auth login` do that means you will not be asked for a password when you push?

**Answer:** `gh auth login` authenticates the GitHub CLI with my GitHub account. It can also configure Git to use the saved authentication, so I do not need to enter my GitHub account password every time I push.

## Question 12

Refresh the repository page on GitHub. What is showing on the front page, and why that file?

**Answer:** The `README.md` file is displayed on the repository's front page as formatted text. GitHub automatically recognizes this standard filename and uses it to introduce the repository.

## Question 13

Run `git log --oneline` again. Did pushing change your local history in any way?

**Answer:** No, pushing did not change my local commit history. It uploaded my existing commits to GitHub so the remote repository could contain them too.

## Question 14

Your repository is private but your TAs can now read it. In your own words, what is the difference between a repository being private and a repository not existing on GitHub at all?

**Answer:** A private repository exists on GitHub but can only be accessed by its owner and people who have been granted permission. A repository that does not exist on GitHub has no hosted repository page or remote content for collaborators to access.
