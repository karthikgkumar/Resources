# su command

While you're logged in to the terminal shell with one user, you might need to switch to another user.

For example you're logged in as root to perform some maintenance, but then you want to switch to a user account.

You can do so with the `su` command:

```bash
su <username>
```

For example: `su flavio`.

If you're logged in as a user, running `su` without anything else will prompt you to enter the `root` user password, as that's the default behavior.

![Screen-Shot-2020-09-03-at-18.18.09](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-18.18.09.png)\
`su` will start a new shell as another user.

When you're done, typing `exit` in the shell will close that shell, and will return you back to the current user's shell.
