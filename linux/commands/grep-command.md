# grep command

### The Linux `grep` command <a href="#the-linux-grep-command" id="the-linux-grep-command"></a>

The `grep` command is a very useful tool. When you master it, it will help you tremendously in your day to day coding.

> If you're wondering, `grep` stands for _global regular expression print_.

You can use `grep` to search in files, or combine it with pipes to filter the output of another command.

For example here's how we can find the occurences of the `document.getElementById` line in the `index.md` file:

```bash
grep -n document.getElementById index.md
```

![Screen-Shot-2020-09-04-at-09.42.10](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-09.42.10.png)

Using the `-n` option it will show the line numbers:

```bash
grep -n document.getElementById index.md
```

![Screen-Shot-2020-09-04-at-09.47.04](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-09.47.04.png)

One very useful thing is to tell grep to print 2 lines before and 2 lines after the matched line to give you more context. That's done using the `-C` option, which accepts a number of lines:

```bash
grep -nC 2 document.getElementById index.md
```

![Screen-Shot-2020-09-04-at-09.44.35](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-09.44.35.png)

Search is case sensitive by default. Use the `-i` flag to make it insensitive.

As mentioned, you can use grep to filter the output of another command. We can replicate the same functionality as above using:

```bash
less index.md | grep -n document.getElementById
```

![Screen-Shot-2020-09-04-at-09.43.15](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-09.43.15.png)

The search string can be a regular expression, and this makes `grep` very powerful.

Another thing you might find very useful is to invert the result, excluding the lines that match a particular string, using the `-v` option:

![Screen-Shot-2020-09-04-at-09.42.04](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-09.42.04.png)
