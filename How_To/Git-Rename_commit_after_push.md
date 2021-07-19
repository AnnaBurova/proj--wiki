# Git: Rename commit after push

```git
> git rebase -i HEAD~n
```

`n` is number of commits behind.

Change `pick` to `r` for those commits that you want to update the message.
Don't bother changing the commit message here, it will be ignored.
You'll do that on the next step.

Type `i` to edit content.

Save and close the editor: `:wq`

Git will pop-up another editor for every revision you put `r` before.
Update the commit message as you like, then save and close the editor.

After all commits messages are updated, you can type `git push -f` to update the remote.
