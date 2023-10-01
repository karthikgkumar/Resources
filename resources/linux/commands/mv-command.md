# mv command

### The Linux `mv` command <a href="#the-linux-mv-command" id="the-linux-mv-command"></a>

Once you have a file, you can move it around using the `mv` command. You specify the file current path, and its new path:

```bash
touch test
mv pear new_pear
```

The `pear` file is now moved to `new_pear`. This is how you **rename** files and folders.

If the last parameter is a folder, the file located at the first parameter path is going to be moved into that folder. In this case, you can specify a list of files and they will all be moved in the folder path identified by the last parameter:

```bash
touch pear
touch apple
mkdir fruits
mv pear apple fruits #pear and apple moved to the fruits folder
```
