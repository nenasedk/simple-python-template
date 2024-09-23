# Tutorial Notes

## git setup
https://docs.github.com/en/get-started/getting-started-with-git

1. Setup git account - login with PERSONAL email address (in case you stop using your Trinity one eventually)
2. What is git? 
    - Repositories, branches, commits, version control,
3. Local setup - `ssh-keygen`
4. Setup username and email
5. git-credential-manager
6. git cheatsheet - basic commands: clone, pull, add, commit, push, merge, status.
7. Best practices: 
    - create branches/forks, make your change (keep it small), and merge back into main.
    - commit often
    - git is NOT a full backup system: don't store large files on the repo. MAKE SURE YOU HAVE ACTUAL BACKUPS.
    - useful commit messages. Keep a changelog, write readmes.
    - document things!
    - Automated workflows (probably too advanced for now, but worth a mention)
8. How to revert to a previous commit
    - https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit
    - `git checkout -b old-state commitid`
    
    This will destroy any local modifications.
    Don't do it if you have uncommitted work you want to keep.
    `git reset --hard commitid`

    Alternatively, if there's work to keep:
    `git stash`
    `git reset --hard commitid`
    `git stash pop`
    This saves the modifications, then reapplies that patch after resetting.
    You could get merge conflicts, if you've modified things which were
    changed since the commit you reset to.



## VS Code Setup
https://code.visualstudio.com/docs/introvideos/basics
1. Download and install
2. Install a few extensions (e.g. python, pylance, jupyter gitlens, pdf, remote)
3. Editing remote code (SSH)
4. Git from within VS Code
5. Tips and tricks
 - keyboard shortcuts
 - autoformatting
 - autosaving
 - Solving merge conflicts
 - breakpoints, variable explorer, debug mode
 - terminal in vs code
 - cells in scripts #%%

## Python Intro
1. Install anaconda - really not recommended to use the installation that came with your computer.
2. Create environments - keep them as compact as possible to avoid conflict between packages.
3. Use an environment in VS Code
4. Installing with pip (normal, local/editable)
5. Installing with conda/conda-forge (occasionally necessary)
6. Try to use as new a version of python as possible (though sometimes things aren't yet compatible with the very newest version)

## Practice
1. Fork https://github.com/nenasedk/simple-python-template/tree/main, 
2. New branch
3. make a change, commit and push. 
4. Merge back into main

## Bonus content
1. Key packages to know: numpy, matplotlib, pandas, scipy, scikit-learn
2. Copilot/AI tools
3. Best Practices
    - Documentation, documentation, documentation (SPHINX if you want to get fancy)
    - Jupyter notebooks vs python models (basic OOP), code structure
    - showyourwork: https://show-your.work/en/latest/
    - organising your directories and projects.
    - naming
    - PEP8
    - testing
    - Packaging (not strictly necessary, but useful if you want other people to use your code)