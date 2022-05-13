# I'm trying to understand the git stage, please correct me

1. git work in 4 stages:
    1. working directory
        ! I created a file say index.html and want to add 4 features
        ! Write some code for feature one, run it, test it all good.
        ! now I move it to staged area.
    2. staged area
        > git add . // this command will move code to staged
    3. Ready to commit area
        > git commit -m "First feature" // this command will read the code for commit.

    Now, I want to add another feature. I will start writing second feature and completed it.
    Now, I will repeat 2nd and 3rd again
    > git add .
    > git commit -m "Second Feature"

    same thing for third feature. after adding my third feature I Realize somthing is wrong Now I want the code which is at the end of first commit.

    I did
    > git checkout "fistCommitNo" "filename"

    I have the code in front of me(in code editor)
    my Head is still Third commit.

    My Que:
    what is this.
    > did I bring all the codes which was at the end of fist commit to unstage area.
    > And is unstage area means my working directory.

    4.remote repositry

2. What I did :
    I added some lines of code to say index.html page
        did the following command:
    > git add .
    > git commit -m "First commit"   // commit id xxxxx1.
    again, I added some few line
        did the following command:
    > git add .
        > git commit -m "Second commit".  // commit id xxxxx2.
    again, I added some few line
        did the following command:
    > git add .
        > git commit -m "third commit".  // commit id xxxxx3.

    my head is xxxxx3.

    if I want the code which was after end of first commit, I will do
    > git checkout xxxxx1 index.html

    now I added some more line
        did the following command:
    > git add .
        > git commit -m "Fourth commit".  // commit id xxxxx4

     my head is xxxxx4.

    **THIS WAY I CAN CHANGE THE VERSION OF CODE**

imp link: "https://blog.codecarrot.net/what-is-difference-between-unstaged-and-untracked-file-in-git"
