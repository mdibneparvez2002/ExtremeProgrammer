# ExtremeProgrammer



## Little docs:
``` bash

git config --global user.email "email"
git config --global user.name " callName / the name the owner knows you"
git add --all
git commit -m "commit message"
git push origin main
git tag -a v0.0.0.1 -m "release message"
git push origin v0.0.0.1

```


# automation script
``` bash
#!/bin/bash

# Define variables
REPO_DIR="/path/to/your/repo"
ZIP_FILE="release_v1.0.0.zip"

### userName & password = "mdibneparvez2002@outlook.com"


git config --global user.email "email"
git config --global user.name " callName / the name the owner knows you"

# Navigate to the repository
cd "$REPO_DIR" || exit

# Add all files
git add --all

# Commit changes
git commit -m "Automated release commit"

# Push to main branch
git push origin main

# Create a ZIP file of the repository
zip -r "$ZIP_FILE" "$REPO_DIR"

# Add ZIP file to Git
git add "$ZIP_FILE"
git commit -m "Added release ZIP file"
git push origin main

echo "Release process completed successfully!"

```




Creating a GitHub Account with a Microsoft Email
Go to GitHub and click Sign Up.

Use your Microsoft email (e.g., yourname@outlook.com or yourname@hotmail.com) to register.

Follow the prompts to verify your email and set up your account.

Creating a Git Repository with Your Microsoft Email
Once you have a GitHub account, you can create a repository:

Sign in to GitHub.

Click the + icon in the top-right and select New Repository.

Choose a name, set visibility (public/private), and click Create Repository.

Setting Your Microsoft Email in Git Locally
If you want to use your Microsoft email for commits:

Open a terminal and run:

sh
git config --global user.email "yourname@outlook.com"
Verify with:

sh
git config --global user.email
This ensures your commits are associated with your Microsoft email.

You can sync files across multiple devices using Git by setting up a remote repository and pulling/pushing changes between devices. Here’s how:

1. Use GitHub, GitLab, or a Private Server
Create a Git repository on a hosting service like GitHub or GitLab.

Clone the repository on each device using:

sh
git clone https://github.com/yourusername/repository.git
Push changes from one device:

sh
git add .
git commit -m "Updated files"
git push origin main
Pull changes on another device:

sh
git pull origin main
2. Sync Without Internet (USB or Local Network)
Set up a bare repository on a USB drive or local server:

sh
git init --bare /path/to/repo.git
Clone it on each device:

sh
git clone /path/to/repo.git
Push and pull changes using the local path.

3. Automate Syncing

Ah, you mean creating releases in Git itself, not GitHub! In Git, releases are typically managed using tags. Here’s how you can do it:

1. Create a Tag for the Release
Tags mark specific points in your repository’s history, often used for releases:

sh
git tag -a v1.0.0 -m "Initial release"
-a creates an annotated tag (recommended for releases).

-m adds a message describing the release.

2. Push the Tag to a Remote Repository
Once you’ve created a tag, push it to your remote repository:

sh
git push origin v1.0.0
This makes the release available to others.

3. List Existing Tags
To see all tags in your repository:

sh
git tag
4. Checkout a Specific Release
If you want to switch to a previous release:

sh
git checkout v1.0.0
5. Delete a Tag (If Needed)
If you need to remove a tag:

sh
git tag -d v1.0.0  # Deletes locally
git push origin --delete v1.0.0  # Deletes remotely

In professional releases, multiple files are added to Git systematically to ensure a clean and organized repository. Here’s how you can do it:

1. Add Specific Files
If you want to add multiple files manually, use:

sh
git add file1.txt file2.txt file3.txt
2. Add All Files in a Directory
To add all files inside a folder:

sh
git add folder_name/*
3. Add All Modified and New Files
To stage all changes, including new and modified files:

sh
git add .
or

sh
git add --all
4. Add Files by Extension
If you want to add all files of a specific type:

sh
git add *.txt
git add *.py
5. Use Interactive Staging
For more control, use interactive staging:

sh
git add -i
This lets you select files individually before committing.

6. Commit with a Structured Message
Once files are staged, commit them with a meaningful message:

sh
git commit -m "Added new features and updated documentation"
Would you like help automating this process for releases? 🚀
