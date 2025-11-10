# Programación 2025 Demo

This is a demonstration repository for using github and integrating with vscode.  This text is written using the online editor github.dev. From the GitHub page of the repository, I opened github.dev by typing `.` (dot). This is a lightweight version of [GitHub Codespaces](https://en.wikipedia.org/wiki/GitHub_Codespaces), which is a more full-featured online IDE.

## Working with a local clone in VS Code

I have cloned it locally by selecting `Continue working in a new local clone` on github.dev

![How to jump from github.dev to local VS Code editor](<CleanShot 2025-11-09 at 12.47.08@2x.png>)

After we edit the files locally, there are four steps we have to go through: 

1. Save the file (`Cmd-S`/`Ctl-S` or `File -> Save` menu item). Now the changes appear in the "Changes" section in Source Control sidebar (this is called your "Working tree" in git, which is all the edits you have made that git does not know about yet). There is also a `File -> Save All` command. Alternatively, you can turn on `Auto Save` so you do not need to worry about this.
2. Stage the changes. Click the `+` button next to the file in the "Changes" section. This is the equivalent of `git add` on the command line. There is also the `Stage Changes` command in the `...` menu in the upper-right corner. These changes now appear in the "Staged Changes" section of the sidebar. 
3. Make a commit using the big blue button. But make sure to write a commit message first that briefly describes your changes. If you have unsaved changes, then you will be warned and given the option to save and stage them first.
4. Push the commit back to GitHub using the big blue button again, which should now say "Sync Changes". 

## Adding another file

* Make sure that we have `uv` installed. Open the integrated terminal and type `uv run python --version`. If it says `Python 3.14.0` then all is good. If it says some other version of python then it is probably finding an existing installation on your machine (avoid this by using `uv run --managed-python python --version`)
* Make a python script `hello.py` and test that it works in the integrated terminal (`uv run hello.py`). Initially the new file `hello.py` appears with a green U because it is "Untracked". Use the "+" button to add it to the staged changes, then write a new commit message, commit and push. 