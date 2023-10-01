# Echo command

### The Linux `echo` command <a href="#the-linux-echo-command" id="the-linux-echo-command"></a>

The `echo` command does one simple job: it prints to the output the argument passed to it.

This example:

```bash
echo "hello"
```

will print `hello` to the terminal.

We can append the output to a file:

```bash
echo "hello" >> output.txt
```

We can interpolate environment variables:

```bash
echo "The path variable is $PATH"
```

![Screen-Shot-2020-09-03-at-15.44.33](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-15.44.33.png)

Beware that special characters need to be escaped with a backslash `\`. `$` for example:

![Screen-Shot-2020-09-03-at-15.51.18](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-15.51.18.png)\
This is just the start. We can do some nice things when it comes to interacting with the shell features.

We can echo the files in the current folder:

```bash
echo *
```

We can echo the files in the current folder that start with the letter `o`:

```bash
echo o*
```

Any valid Bash (or any shell you are using) command and feature can be used here.

You can print your home folder path:

```bash
echo ~
```

![Screen-Shot-2020-09-03-at-15.46.36](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-15.46.36.png)

You can also execute commands, and print the result to the standard output (or to file, as you saw):

```bash
echo $(ls -al)
```

![Screen-Shot-2020-09-03-at-15.48.55](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-15.48.55.png)

Note that whitespace is not preserved by default. You need to wrap the command in double quotes to do so:

![Screen-Shot-2020-09-03-at-15.49.53](https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-15.49.53.png)

You can generate a list of strings, for example ranges:

```bash
echo {1..5}

```

<figure><img src="https://www.freecodecamp.org/news/content/images/2020/10/Screen-Shot-2020-09-03-at-15.47.19.png" alt=""><figcaption></figcaption></figure>
