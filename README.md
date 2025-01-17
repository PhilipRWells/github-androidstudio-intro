# BIT 300: Get-Set Mobile Github and Android Studio
## GIT basics and Best Practices

1. Why Git?

   * There are other version control systems. There are a number of Version Control Systems out there. This alone should prove that version control is incredibly important. Examples

     * [Git](https://git-scm.com)
     * [Subversion](https://subversion.apache.org)
     * [Mercurial](https://www.mercurial-scm.org)

    * Git is the most popular and an industry standard.

   * It has some advantages over a centralized system, which has a single copy of the code:

     * It's quick to take action on your own copy
     * It works locally, on your own computer, and offline
     * It makes having multiple branches, parallel worlds of code, easier

     ![git workflow steps](./GitWorkFlow.gif)

2. Git Gotchas

   * Git can mean several things - the name of the source control technology, the functionality built into VS Code, the file formats and protocols that underlie the system.
   * It’s both powerful (because it’s open-ended), plentiful (because it’s open source), and sometimes hard to use (because it’s open-ended).
   * It takes practice, it's a learned skill, it's not intuitive - ask other developers about their Git disasters - everyone has a story.


## Git Demo Using Git Bash/ Android Studio Terminal

1. Creating new repo and initial commit. The flow for using git starts with creating a directory (folder). The cycle as changes are made is `add` and `commit`. Record your changes in small chunks as you go.

   * Configure your git
     * `git config --global user.email "youremail"`
     * `git config --global user.name "yourname"`
   * `mkdir SampleApp` - create new folder named SampleApp
   * `cd SampleApp` - move to the project folder
   * `git init` - initialize the repository
   * `touch README.md` - create a new file
   * `git status` - view the repository status
   * `git add  .` - stage the files to commit and tell get what files to track, "." selects all the new files or files with changes
   * `git commit README.md -m "New readme file"` - add the changes to the repo with the named file, "-m" indicates message included


## Demo: Git using Android Studio's VCS menu

1. Create a new "Empty Activity" project in Android Studio and use the built-in git support (*VCS menu*). It doesn't have all the commands of Git Bash or the command line but is convenient when working in Android Studio.

2. Add a TEXT file called "myFile" (File/New/File)

3. Use "*VCS > Enable Version Control Integration*" to initialize a repository - choose "Git" as your VCS

4. Follow the git workflow 

   * **View the repository status**: using "*Git>Commit*" from the menu
   * **Stage the files to commit**: select the "myFile" doc from the list (find it in the *Unversioned Files* list)
   * **Commit the changes with a comment**: Type a commit message in the box, like "tests commit process in Android Studio" and click "Commit"

5. Review the effect using the Terminal

   * Open the "Terminal" tab "*View > Tool Windows > Terminal*"
   * Check out the changes with `git log`
   * See the difference between `git log` and `git log --oneline`

## Work with Remote GitHub repositories
### use the Canvas document to complete the exercise with a partner
1. Fork and Clone this GitHub repository
3. Use both the terminal and Android Studio to work with Git
4. Push your changes to GitHub
5. Submit the URL for your updated repo in Canvas
