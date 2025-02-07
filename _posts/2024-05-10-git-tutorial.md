---
layout: tutorial
title: "Git Versioning"
session: 4
tags: [4,tutorial]
category: tutorial
image: git.svg
---

### 1. Getting started

1. Download and install [GitHub Desktop](https://desktop.github.com/). When it asks for your username and password, press "skip". For "name" and "email address" you can give anything you don't mind showing up publicly (a pseudonym or junk email address is fine).
2. Clone the project/repository <https://gitlab.gwdg.de/24recipes/24recipes.pages.gwdg.de>
    <video width="450" controls>
    <source src="../assets/img/git-clone-repository.mov" type="video/mp4">
    </video> 

### 2. Syncing and editing files

1. In GitHub Desktop, create a new branch.
    <video width="450" controls>
        <source src="../assets/img/git-new-branch.mov" type="video/mp4">
    </video> 

2. Open the project/repository in Visual Studio Code.
3. Edit one of the files in `_posts` or create a new one with the name and date, such as `2024-05-06-cookies.md`
    <video width="450" controls>
    <source src="../assets/img/git-new-branch.mov" type="video/mp4">
    </video> 
If you're feeling confident and would like to try creating a new file, you can do so by making another file in the `_posts` directory, named the same way, with the date (YYYY-MM-DD) and then a name and the `.md` extension.  
    <video width="450" controls>
        <source src="../assets/img/git-new-file.mov" type="video/mp4">
    </video> 

4. Commit changes and publish your branch (using the password in [OLAT](https://olat-ce.server.uni-frankfurt.de/olat/auth/RepositoryEntry/20670545926/CourseNode/1713408124938163007) and any username).

    <video width="450" controls>
        <source src="../assets/img/git-sync-changes.mov" type="video/mp4">
    </video> 

###  3. Setting up an account in Gitlab GWDG

1. Log into <https://academiccloud.de/> using "Federated Login" > "Universität Frankfurt". 
2. After you're logged in, go to <https://id.academiccloud.de/account>. Copy the "username" and "Academic ID" that appears there and send them to me. I'll request access for you. 
3. Once I let you know you have access, sign in at <https://gitlab.gwdg.de/users/sign_in?redirect_to_referer=yes>. 

###  4. Creating a merge request

**Note:** You will only be able to do this step once GWDG has granted you access to Gitlab.

1. Go to the project <https://gitlab.gwdg.de/24recipes/24recipes.pages.gwdg.de>. 
2. Click on "Sign in" at the top right of the screen. Click "Federated Login" > "Universität Frankfurt" and login with your HRZ account as before.
3. At the top left, under the title "Recipes," change the branch from `master` to the one you created. 
4. On the top right, click "Compare." (The Source will be set as your branch and the Target should say "master".)
5. Click "Create Merge Request," then scroll to the bottom of the new page and click "Create Merge Request" again. I will be able to see and approve the merge request. Once I do, your changes will appear on the website at <https://24recipes.pages.gwdg.de/>.

<video width="450" controls>
    <source src="../assets/img/git-merge-request.mov" type="video/mp4">
</video> 
