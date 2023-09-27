# Emacs Editor

### The Linux `emacs` editor command <a href="#the-linux-emacs-editor-command" id="the-linux-emacs-editor-command"></a>

`emacs` is an awesome editor and it's historically regarded as _the_ editor for UNIX systems. Famously, `vi` vs `emacs` flame wars and heated discussions have caused many unproductive hours for developers around the world.

`emacs` is very powerful. Some people use it all day long as a kind of operating system ([https://news.ycombinator.com/item?id=19127258](https://news.ycombinator.com/item?id=19127258)). We'll just talk about the basics here.

You can open a new emacs session simply by invoking `emacs`:

![Screenshot-2019-02-10-at-12.14.18](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-12.14.18.png)

> macOS users, stop a second now. If you are on Linux there are no problems, but macOS does not ship applications using GPLv3, and every built-in UNIX command that has been updated to GPLv3 has not been updated.
>
> While there is a little problem with the commands I listed up to now, in this case using an emacs version from 2007 is not exactly the same as using a version with 12 years of improvements and change.
>
> This is not a problem with Vim, which is up to date. To fix this, run `brew install emacs` and running `emacs` will use the new version from Homebrew (make sure you have [Homebrew](https://flaviocopes.com/homebrew/) installed).

You can also edit an existing file by calling `emacs <filename>`:

![Screenshot-2019-02-10-at-13.12.49](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-13.12.49.png)

You can now start editing. Once you are done, press `ctrl-x` followed by `ctrl-w`. You confirm the folder:

![Screenshot-2019-02-10-at-13.14.29](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-13.14.29.png)

and Emacs tells you the file exists, asking you if it should overwrite it:

![Screenshot-2019-02-10-at-13.14.32](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-13.14.32.png)

Answer `y`, and you get a confirmation of success:

![Screenshot-2019-02-10-at-13.14.35](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-13.14.35.png)\
You can exit Emacs by pressing `ctrl-x` followed by `ctrl-c`.\
Or `ctrl-x` followed by `c` (keep `ctrl` pressed).

There is a lot to know about Emacs, certainly more than I am able to write in this little introduction. I encourage you to open Emacs and press `ctrl-h` `r` to open the built-in manual and `ctrl-h` `t` to open the official tutorial.
