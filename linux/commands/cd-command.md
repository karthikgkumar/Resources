# cd command

### The Linux `cd` command <a href="#the-linux-cd-command" id="the-linux-cd-command"></a>

Once you have a folder, you can move into it using the `cd` command. `cd` means **c**hange **d**irectory. You invoke it specifying a folder to move into. You can specify a folder name, or an entire path.

Example:

```bash
mkdir fruits
cd fruits
```

Now you are in the `fruits` folder.

You can use the `..` special path to indicate the parent folder:

```bash
cd .. #back to the home folder
```

The # character indicates the start of the comment, which lasts for the entire line after it's found.

You can use it to form a path:

```bash
mkdir fruits
mkdir cars
cd fruits
cd ../cars
```

There is another special path indicator which is `.`, and indicates the **current** folder.

You can also use absolute paths, which start from the root folder `/`:

```bash
cd /etc
```
