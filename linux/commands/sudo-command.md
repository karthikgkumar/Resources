# sudo command

`sudo` is commonly used to run a command as root.

You must be enabled to use `sudo`, and once you are, you can run commands as root by entering your user's password (_not_ the root user password).

The permissions are highly configurable, which is great especially in a multi-user server environment. Some users can be granted access to running specific commands through `sudo`.

For example you can edit a system configuration file:

```bash
sudo nano /etc/hosts
```

which would otherwise fail to save since you don't have the permissions\
for it.

You can run `sudo -i` to start a shell as root:

![Screen-Shot-2020-09-03-at-18.25.50](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-18.25.50.png)

You can use `sudo` to run commands as any user. `root` is the default, but use the `-u` option to specify another user:

```bash
sudo -u flavio ls /Users/flavio
```
