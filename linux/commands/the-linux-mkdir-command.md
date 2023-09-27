# The Linux mkdir command

You create folders using the `mkdir` command:

```bash
mkdir fruits
```

You can create multiple folders with one command:

```bash
mkdir dogs cars
```

You can also create multiple nested folders by adding the `-p` option:

```bash
mkdir -p fruits/apples
```

Options in UNIX commands commonly take this form. You add them right after the command name, and they change how the command behaves. You can often combine multiple options, too.

You can find which options a command supports by typing `man <commandname>`. Try now with `man mkdir` for example (press the `q` key to esc the man page). Man pages are the amazing built-in help for UNIX.
