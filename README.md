# GitSteps 🐙

#### Project in Progress ⚠️

### Step by step: how to use Git with GitHub for beginners

<img><center>

![image](https://user-images.githubusercontent.com/100430135/182463113-50b296fb-b67f-4e1e-a986-4fc2c610e357.png)

</center></img>

### Prerequisites ⚠️
- Git
- A GitHub account

---

In this short tutorial, I'll show you how to use Git basics for your projects and code versioning. This includes:

- Clone
- Init
- Commit
- Push
- Pull

<br>

## Step 1 — Download Git

First, you'll need to have Git installed on your machine. If you don't already have it, click here -> [Download Git](https://git-scm.com/), then download and install it.

<br>

![GitSite](https://user-images.githubusercontent.com/100430135/184555032-982838bb-8cae-4641-9729-f624d10de1dc.png)

<br>

---

<br>

## Step 2 — Create or access a GitHub account

If you don't have a GitHub account yet, go to the official website or click here -> [GitHub](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) to be redirected to the sign-up page. You can log in to an existing account or create a new one.

<br>

![GithubSite](https://user-images.githubusercontent.com/100430135/184555266-9e8e631f-6391-455e-b006-7812e5fdb547.png)

<br>

---

<br>

## Step 3 — Create a repository on GitHub

After creating your GitHub account, go to the "Repositories" tab at the top of the page, next to "Projects", and click the "New" button. You'll be taken to a page where you can set up your repository, choosing options such as name, description, and visibility.

<br>

![NewRepository](https://user-images.githubusercontent.com/100430135/184555470-97a3931d-468d-4ebd-ba19-d5b2e32bfc2c.png)

<br>

Choose a name for your repository — mine will be called `gitSteps`.

If you'd like other people, such as classmates or recruiters, to be able to see this repository, keep the "Public" option selected. If it's a private project, choose "Private" instead.

It's also a good idea to leave the "Add a README file" option checked, since the README acts as the cover page of your repository — it's where you'll describe its purpose, usage instructions, and key features.

Once you've made your choices, create your remote repository by clicking "Create repository".

<br>

---

<br>

## Step 4 — Clone the remote repository to your computer

Inside the repository you just created, click the green "Code" button. You'll see an HTTPS link that points to the remote repository — this is what we'll use to clone it to your local machine. Save this link, it's important.

<br>

![GitClone1](https://user-images.githubusercontent.com/100430135/184555763-b711175c-6e6b-467e-9a77-c8fe6140aec6.png)

<br>

Create a folder on your computer where you'll keep the files you're going to work on. It can be on the desktop or anywhere else you like — mine will be on the desktop. Give the folder a meaningful name; for my projects, I usually call mine "Git".

<br>

![PastaGit1](https://user-images.githubusercontent.com/100430135/184556009-2d64d691-26e0-4ecd-8e94-95ceb42cf408.png)

![PastaGit2](https://user-images.githubusercontent.com/100430135/184556010-0a92750d-fdd0-42ed-9d2c-0aad4c82d382.png)

<br>

Open the folder, right-click inside it, and — if you already have Git installed — select "Git Bash Here". This opens the Git terminal (Bash), which works via command line, and it's what we'll use to version our code and projects.

<br>

![GitBashHere](https://user-images.githubusercontent.com/100430135/184556106-4692af03-4974-4968-9e64-0a96d4b720dc.png)

<br>

With Bash (the Git terminal) open, type the command <span style="color:red">git clone + repository link</span>.

The link you use should be the one from your remote repository — the one you just created on GitHub and saved earlier. Use it with the command <span style="color:red">git clone + link</span>.

<br>

![gitClone2](https://user-images.githubusercontent.com/100430135/184556271-7197e926-7261-41d0-9e19-33eb1969304e.png)

<br>

After running this command, Git will download a copy of the remote repository into the local folder you created, where you'll be able to work on your code and projects.

<br>

![2022-08-14 (12)](https://user-images.githubusercontent.com/100430135/184558866-12684abd-bf5c-45bc-b153-aa9ccf91b375.png)

<br>

---

<br>

## Step 5 — Add the files for your project

With the repository already cloned into your local folder, add the files that will make up your project — for example:
- index.html
- wallpaper.png
- style.css

<br>

![gitAdd1](https://user-images.githubusercontent.com/100430135/184556873-d8a70027-84f0-4dfb-911e-2abcf620151f.png)

<br>

Once your files are inside the folder (for example, if you created them from VS Code, which is possible and recommended), open the Git Bash terminal and type the command <span style="color:red">git add .</span>

This command stages all the files in the folder for versioning, meaning they're now ready to be committed and pushed to GitHub.

<br>

![gitAdd2](https://user-images.githubusercontent.com/100430135/184556969-ed5f7234-b7ed-4ff1-9054-30ac1de04345.png)

<br>

I used the command <span style="color:red">git status</span> to check the status of the new files in the local repository folder.

<br>

![gitAdd3](https://user-images.githubusercontent.com/100430135/184556968-225e71da-ed63-4e9d-a3b1-ddc7915bc013.png)

<br>

---

<br>

## Step 6 — The commit command

The commit command saves the current state of your staged files as a new version, along with a short description. In other words, a commit marks the completion of a set of changes — the next step after committing is to push those changes to the remote repository on GitHub.

The syntax for the commit command is <span style="color:red">git commit -m "message"</span>. The `-m` flag expects a message, placed inside quotes (" "), which briefly describes your update. For example:

- `git commit -m "add new features"`
- `git commit -m "add new header"`
- `git commit -m "add new image to site"`

<br>

![gitCommit1](https://user-images.githubusercontent.com/100430135/184557179-102e3aad-d6f3-4cfe-acb4-f908e4e5e96a.png)

<br>

After running this command, the terminal will display messages showing which files were committed.

<br>

![gitCommit2](https://user-images.githubusercontent.com/100430135/184557178-e7e7bc9c-d9b2-4cec-96ab-1b412ff4038f.png)

<br>

---

<br>

## Step 7 — The push command and GitHub

Now, finally, it's time to send your files to GitHub using the push command. The <span style="color:red">git push</span> command uploads all the latest updates from your local repository to GitHub, keeping your remote repository in sync with your local one after every push.

<br>

![gitPush1](https://user-images.githubusercontent.com/100430135/184557609-3257405c-ef47-44eb-9d6a-6b8ee8fa1969.png)

<br>

After running <span style="color:red">git push</span>, the terminal will display messages confirming that the push was completed successfully.

<br>

![gitPush2](https://user-images.githubusercontent.com/100430135/184557610-61b6c998-42f6-4e42-924b-15735cb3254a.png)

<br>

After pushing, go to your GitHub account and you'll see that your repository has been updated with the files from your computer. From now on, whenever you want to add a new file or modify an existing one, just repeat the cycle:

1. `git add .`
2. `git commit -m "message"`
3. `git push`

---

<br>