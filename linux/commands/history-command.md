# History command

Every time you run a command, it's memorized in the history.

You can display all the history using:

```bash
history
```

This shows the history with numbers:

![Screen-Shot-2020-09-04-at-08.03.10](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-08.03.10.png)

You can use the syntax `!<command number>` to repeat a command stored in the history. In the above example typing `!121` will repeat the `ls -al | wc -l` command.

Typically the last 500 commands are stored in the history.

You can combine this with `grep` to find a command you ran:

```bash
history | grep docker
```

![Screen-Shot-2020-09-04-at-08.04.50](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-08.04.50.png)\
To clear the history, run `history -c`.
