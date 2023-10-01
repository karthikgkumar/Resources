# Vim Editor

### The Linux `vim` editor command <a href="#the-linux-vim-editor-command" id="the-linux-vim-editor-command"></a>

`vim` is a **very** popular file editor, especially among programmers. It's actively developed and frequently updated, and there's a big community around it. There's even a [Vim conference](https://vimconf.org/)!

`vi` in modern systems is just an alias for `vim`, which means `vi` i`m`proved.

You start it by running `vi` on the command line.

![Screenshot-2019-02-10-at-11.44.36](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-11.44.36.png)

You can specify a filename at invocation time to edit that specific file:

```bash
vi test.txt
```

![Screenshot-2019-02-10-at-11.36.21](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-11.36.21.png)

You have to know that Vim has 2 main modes:

* _command_ (or _normal_) mode
* _insert_ mode

When you start the editor, you are in command mode. You can't enter text like you expect from a GUI-based editor. You have to enter **insert mode**.

You can do this by pressing the `i` key. Once you do so, the `-- INSERT --` word appears at the bottom of the editor:

![Screenshot-2019-02-10-at-11.47.39](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-11.47.39.png)

Now you can start typing and filling the screen with the file contents:

![Screenshot-2019-02-10-at-11.48.39](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-11.48.39.png)

You can move around the file with the arrow keys, or using the `h` - `j` - `k` - `l` keys. `h-l` for left-right, `j-k` for down-up.

Once you are done editing you can press the `esc` key to exit insert mode and go back to **command mode**.

![Screenshot-2019-02-10-at-11.48.44](https://www.freecodecamp.org/news/content/images/2020/10/Screenshot-2019-02-10-at-11.48.44.png)\
At this point you can navigate the file, but you can't add content to it (and be careful which keys you press, as they might be commands).

One thing you might want to do now is **save the file**. You can do so by pressing `:` (colon), then `w`.

You can **save and quit** by pressing `:` then `w` and `q`: `:wq`

You can **quit without saving** by pressing `:` then `q` and `!`: `:q!`

You can **undo** and edit by going to command mode and pressing `u`. You can **redo** (cancel an undo) by pressing `ctrl-r`.

Those are the basics of working with Vim. From here starts a rabbit hole we can't go into in this little introduction.

I will only mention those commands that will get you started editing with Vim:

* pressing the `x` key deletes the character currently highlighted
* pressing `A` goes to the end of the currently selected line
* press `0` to go to the start of the line
* go to the first character of a word and press `d` followed by `w` to delete that word. If you follow it with `e` instead of `w`, the white space before the next word is preserved
* use a number between `d` and `w` to delete more than 1 word, for example use `d3w` to delete 3 words forward
* press `d` followed by `d` to delete a whole entire line. Press `d` followed by `$` to delete the entire line from where the cursor is, until the end

To find out more about Vim I can recommend the [Vim FAQ](https://vimhelp.org/vim\_faq.txt.html). You can also run the `vimtutor` command, which should already be installed in your system and will greatly help you start your `vim` exploration.
