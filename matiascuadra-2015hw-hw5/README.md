# 2015hw

You MAY NOT share this repository to the public.

Let me describe the steps by which you gain access to the homework.

1. Our read-only repository is `cs109-students/2015hw`. All students have read-only access to this repository. You can see this homework there under the "hw5" branch. Any changes after the homework has gone out will be made here.
2. You will have your own read-write repository under the `cs109-students` organization, which will be of the form`cs109-students/githubusername-2015hw`. Only you and the cs109 staff have access to this repository, thus ensuring the privacy of your homework.
3. This homework is on the hw5 branch. There is `master` branch too, which will have some instructions, but nothing very exciting. You will never work on this branch.

On the assumption that you followed the appropriate flow for the hw0 branch and have a master and a hw0, hw1, hw2, hw3, and hw4 branch currently on your computer, this is what you do:

1. First make sure you have submitted hw4 by pushing it, and checking it has been submitted on the web interface. Also copy your hw3.ipynb SOMEWHERE ELSE on your machine, just to be safe.
2. **FIRST MAKE SURE YOU ARE ON MASTER** by doing `git checkout master` inside your `githubusername-2015hw` folder
3. Do `git fetch origin hw5`, which fetches from *your* remote repository (named `origin`) on github the `hw5`branch. Then you issue `git checkout -b hw5 origin/hw5`. This command makes a new local branch `hw5` on your machine which tracks the `hw5` branch on your remote.
4. You are now in the `hw5` branch. This is where you will work on homework 5. Start/Open the ipython notebooks in the repository and run the homework. The files you will use is `hw5part1.ipynb` and `hw5part2.ipynb`. The first one uses Spark and will need to be opened in the way you worked on Spark notebooks in section. You may run it directly on your machine (Mac Homebrew users), on Vagrant, or on AWS. DO NOT run the notebooks ending in`_original.ipynb`. These are simply copies of the homework. We made these copies so that you can update them from our `course` remote in case we make any changes. You will now engage in the "edit/add/commit/push" cycle as described above. (The `push` will only push to the remote `hw5` branch.)
5. This homework is due Thursday, November 19th 2015, at 11:59PM EST.
We'll grade the last commit you make before the homework deadline. We will be looking for the files hw5part1.ipynb, hw5part2.ipynb, and dftouse.csv.

Once again, in case we make changes, you can incorporate them into your repo by doing: `git fetch course; git checkout course/hw5 -- hw5_original.ipynb`. An "add/commit/push" cycle will make sure these changes go into your fork as well. If you have already started working, it might be easiest to manually copy the changes into hw5part1.ipynb or hw5part2.ipynb. Remember, thats the file we are looking for, NOT, `hw5_original.ipynb`

If you are an advanced git user, it might be safer for you to create a branch off the hw5 branch, like say, play-hw5, and work there. You can then merge it in.
