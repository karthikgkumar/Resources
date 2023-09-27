# find command

### The Linux `find` command <a href="#the-linux-find-command" id="the-linux-find-command"></a>

The `find` command can be used to find files or folders matching a particular search pattern. It searches recursively.

Let's learn how to use it by example.

Find all the files under the current tree that have the `.js` extension and print the relative path of each file that matches:

```bash
find . -name '*.js'
```

It's important to use quotes around special characters like `*` to avoid the shell interpreting them.

Find directories under the current tree matching the name "src":

```bash
find . -type d -name src
```

Use `-type f` to search only files, or `-type l` to only search symbolic links.

`-name` is case sensitive. use `-iname` to perform a case-insensitive search.

You can search under multiple root trees:

```bash
find folder1 folder2 -name filename.txt
```

Find directories under the current tree matching the name "node\_modules" or 'public':

```bash
find . -type d -name node_modules -or -name public
```

You can also exclude a path using `-not -path`:

```bash
find . -type d -name '*.md' -not -path 'node_modules/*'
```

You can search files that have more than 100 characters (bytes) in them:

```bash
find . -type f -size +100c
```

Search files bigger than 100KB but smaller than 1MB:

```bash
find . -type f -size +100k -size -1M
```

Search files edited more than 3 days ago:

```bash
find . -type f -mtime +3
```

Search files edited in the last 24 hours:

```bash
find . -type f -mtime -1
```

You can delete all the files matching a search by adding the `-delete` option. This deletes all the files edited in the last 24 hours:

```bash
find . -type f -mtime -1 -delete
```

You can execute a command on each result of the search. In this example we run `cat` to print the file content:

```bash
find . -type f -exec cat {} \;
```

Notice the terminating `\;`. `{}` is filled with the file name at execution time.
