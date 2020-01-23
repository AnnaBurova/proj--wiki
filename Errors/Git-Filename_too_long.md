# Git checkouts fail on Windows with "Filename too long error: unable to create file"

Filename too long, comes from a Windows API limitation of file paths having 260 characters or fewer.

## Resolution

To resolve this issue, please run the following command from GitBash or the Git CMD prompt:

```
git config --system core.longpaths true
```

This will allow file paths of 4096 characters.
