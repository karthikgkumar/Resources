# Cat command

### The Linux `cat` command <a href="#the-linux-cat-command" id="the-linux-cat-command"></a>

Similar to [`tail`](https://www.freecodecamp.org/news/unix-command-tail/) in some ways, we have `cat`. Except `cat` can also add content to a file, and this makes it super powerful.

In its simplest usage, `cat` prints a file's content to the standard output:

```bash
cat file
```

You can print the content of multiple files:

```bash
cat file1 file2
```

and using the output redirection operator `>` you can concatenate the content of multiple files into a new file:

```bash
cat file1 file2 > file3
```

Using `>>` you can append the content of multiple files into a new file, creating it if it does not exist:

```bash
cat file1 file2 >> file3
```

When you're looking at source code files it's helpful to see the line numbers. You can have `cat` print them using the `-n` option:

```bash
cat -n file1
```

You can only add a number to non-blank lines using `-b`, or you can also remove all the multiple empty lines using `-s`.

`cat` is often used in combination with the pipe operator `|` to feed a file's content as input to another command: `cat file1 | anothercommand`.
