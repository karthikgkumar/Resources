# passwd command

Users in Linux have a password assigned. You can change the password using the `passwd` command.

There are two situations here.

The first is when you want to change your password. In this case you type:

```bash
passwd
```

and an interactive prompt will ask you for the old password, then it will ask you for the new one:

![Screen-Shot-2020-09-04-at-07.32.05](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-04-at-07.32.05.png)

When you're `root` (or have superuser privileges) you can set the username for which you want to change the password:

```bash
passwd <username> <new password>
```

In this case you don't need to enter the old one.
