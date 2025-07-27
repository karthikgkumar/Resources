# rm Command


### The Linux `rm` Command

The `rm` command is used to **remove files or directories**.  
Once you remove something with `rm`, it is **permanently deleted** (not moved to trash), so use it carefully.

To remove a **file**, simply specify the filename:

```bash
rm file.txt
````

You can remove multiple files at once:

```bash
rm file1.txt file2.txt
```

If you try to remove a **directory**, you must use the `-r` (recursive) option:

```bash
rm -r myfolder
```

This will delete the folder `myfolder` and **all of its contents**, including subfolders and files.

To avoid confirmation prompts when deleting, you can add the `-f` (force) option:

```bash
rm -rf myfolder
```

**Warning:**
`rm -rf` is very powerful—**double-check your path** before executing this command.
Running `rm -rf /` or `rm -rf *` in the wrong directory can wipe your entire system.

---

You can also use the `-v` option for verbose output, to see which files are being removed:

```bash
rm -rv old_directory
```

The `#` character starts a comment, which lasts to the end of the line:

```bash
rm -rf myfolder  # Remove the folder and all its contents without confirmation
```

---

### Example: Create and remove directories

```bash
mkdir fruits
mkdir cars
rm -r fruits
```

This creates two folders, then deletes `fruits` and everything inside it (if any).

---
### Remove Git Tracking by Deleting .git Folder
To stop Git from tracking a project, delete the .git directory:

```
rm -rf .git
```
⚠️ Warning:
- This permanently removes all Git history and config.
- It does not delete your project files.
- Use with caution — make backups if needed.
---
To learn more, check the manual:

```bash
man rm
```

