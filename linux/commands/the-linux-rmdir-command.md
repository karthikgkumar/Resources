# The Linux rmdir command

Just as you can create a folder using `mkdir`, you can delete a folder using `rmdir`:

```bash
mkdir fruits
rmdir fruits
```

You can also delete multiple folders at once:

```bash
mkdir fruits cars
rmdir fruits cars
```

The folder you delete must be empty.

To delete folders with files in them, we'll use the more generic `rm` command which deletes files and folders, using the `-rf` option:

```bash
rm -rf fruits cars
```

Be careful as this command does not ask for confirmation and it will immediately remove anything you ask it to remove.

There is no **bin** when removing files from the command line, and recovering lost files can be hard.
