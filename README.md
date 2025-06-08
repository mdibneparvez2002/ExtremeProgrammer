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







sync across devices:
Today
best cli based editor / ide for 2050
Predicting the best CLI-based editor or IDE for 2050 is a bit of a stretch, but based on current trends, some of the most powerful terminal editors today include Neovim, Vim, Kakoune, and Micro.

Neovim, for example, is a modernized fork of Vim that aims to improve extensibility while keeping the efficiency of its predecessor. Meanwhile, Micro is a beginner-friendly terminal editor with seamless system clipboard integration and multi-cursor support1.

If you're looking for something futuristic, AI-powered coding assistants integrated into CLI editors might become the norm by 2050. What features would you want in a next-gen terminal editor? 🚀





Edit this response
What features do current CLI editors lack?
Current CLI editors have come a long way, but they still have some limitations. Here are a few areas where they could improve:

Better Default Options: Some operating systems, like Windows, lack a built-in CLI editor by default, requiring users to install one manually.

Intuitive User Experience: Many CLI editors have a steep learning curve, especially modal editors like Vim. New users often struggle with basic commands, such as exiting the editor.

Modern UI Features: While CLI editors prioritize efficiency, they often lack features like mouse support, multi-file tabs, and rich text formatting.

Extensibility & Plugin Support: Some editors have limited plugin ecosystems, making it harder to customize workflows.

Better Error Handling: Some CLI editors could improve error messages and recommendations when commands fail due to missing packages.

Would you like to explore futuristic CLI editor concepts? 🚀





Edit this response
what about emacs
Ah, Emacs—the legendary editor that’s practically an operating system disguised as a text editor! 😆

Emacs is known for its extensibility, allowing users to customize nearly every aspect of their workflow using Emacs Lisp. Some standout features include:

Content-aware editing with syntax highlighting for various file types.

Built-in documentation and a tutorial for new users.

Full Unicode support for almost all human scripts.

Highly customizable via Lisp or graphical interfaces.

Beyond text editing—it can function as a project planner, mail reader, debugger, IRC client, and more.

Package management system for installing extensions.

The latest version, Emacs 30.1, was released in February 2025, bringing improvements like native compilation enabled by default, Android support, touchscreen enhancements, and Tree-Sitter modes for multiple languages.

Would you consider switching to Emacs, or are you more of a Vim/Neovim person? 😏





Edit this response
and what about microdoft edit cli?
Microsoft Edit is a new command-line text editor for Windows, designed to be lightweight and user-friendly. It pays homage to the classic MS-DOS Editor but introduces modern features like mouse support, multi-file editing, find & replace, and word wrap2.

Unlike modal editors like Vim, Edit is modeless, meaning users don’t have to switch between different modes to perform actions. It’s also open-source, available on GitHub, and can be installed via WinGet.

Would you consider using Edit, or do you prefer more established CLI editors like Vim or Emacs? 😏





Edit this response
so how can I show tabs opened as other editors do in ms edit?
In Microsoft Edit, you can open multiple files and switch between them, but it doesn’t display tabs like GUI-based editors. Instead, it uses a file list in the lower-right corner of the interface, and you can switch between open files using Ctrl+P.

If you’re looking for a more traditional tabbed experience, you might want to use Windows Terminal panes, which allow you to run multiple command-line applications side by side. While this isn’t exactly the same as tabs in an editor, it can help you manage multiple files efficiently.

Would you like to explore other ways to enhance your workflow in Edit? 🚀





Edit this response
What other features can improve my workflow in MS Edit?
Microsoft Edit has some great features, but there are ways to enhance your workflow even further. Here are a few improvements you might find useful:

Keyboard Shortcuts: Edit supports shortcuts like Ctrl+P for switching files and Ctrl+R for find & replace.

Mouse Mode Support: Unlike many CLI editors, Edit allows mouse interaction, making navigation easier.

Word Wrap & Regular Expressions: You can enable word wrap with Alt+Z and use regex-based search for advanced text manipulation.

Customization & Open Source Contributions: Since Edit is open-source, you can tweak its behavior or contribute to its development on GitHub.

Windows Terminal Integration: Running Edit inside Windows Terminal allows you to use split panes for multitasking.

Would you like to explore specific customization options? 🚀





Edit this response
can I customize ms edit?
Yes! Microsoft Edit is open-source, meaning you can customize it to fit your workflow. Here are some ways to tweak it:

Modify Keybindings: Since Edit is modeless, you can adjust shortcuts to match your preferences.

Enable Mouse Mode: You can toggle mouse support for easier navigation.

Customize Appearance: Edit allows basic UI tweaks, such as adjusting colors and fonts.

Extend Functionality: Since it's built with Rust, developers can contribute to its GitHub repository and add new features.

Install via WinGet: You can install the latest version using winget install Microsoft.Edit.

If you're interested in deeper customization, you can check out the official GitHub repository or the Microsoft Dev Blog. 🚀 Would you like help setting up specific configurations?





Edit this response
how to create a git repo with ms outlook
Microsoft Outlook isn't designed for Git repository management, but you can integrate GitHub with Outlook using automation tools like n8n. This allows you to create workflows that connect GitHub repositories with Outlook emails, notifications, or task management.

If you're looking to send Git patches via email, you can configure git send-email to work with Outlookgit send-emailto work with Outlook. This requires setting up an SMTP server that supports OAuth authentication.

Would you like help setting up GitHub automation with Outlook? 🚀





Edit this response
i mean create a github repo with microsoft email, but create git repo with the ms email.
You can absolutely create a GitHub repository using your Microsoft email! Here’s how:

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

Would you like help setting up SSH keys or authentication for GitHub? 🚀

how to sync files across my devices using git?
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
Use Git hooks to automatically push changes when committing.

Set up cron jobs or Windows Task Scheduler to pull updates periodically.

Would you like help setting up a specific sync method? 🚀



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
Would you like help automating releases with scripts? 🚀


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
