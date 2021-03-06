# Step 7: The joe Editor

There are many editors available for use on the character-based shell interface. Editors like `vi`, `vim`, `nano`, and `joe`. Compare these to 5250 editors like `SEU` or `EDTF`.

For the purposes of this lab we will focus on the [`joe`](http://joe-editor.sourceforge.net/) editor because it works well in PASE whereas `vi` doesn't.

To edit a file with `joe` simply enter the following.

```text
~% joe file.txt
```

Your shell should then look like the following screenshot.

![](.gitbook/assets/joe_editor_filedottxt.png)

You are now in a live editor that will allow you to modify the contents of `file.txt`. Add the following lines as content in `file.txt`.

```text
hi, I am on line 1 line 2 3rd is best
```

Now it's time to save the file and close the editor. This is where keyboard shortcuts become very important because these character editors don't usually work with a mouse. To learn what the keyboard shortcuts are press `Ctrl` + `KH` to bring up the `joe` editor's Help Screen, as shown below.

**NOTE:** Pressing `Ctrl` + `K` puts it into a special mode where it awaits an additional modifier \(`H` in this example\) to know what to do next.

![](.gitbook/assets/joe_editor2_help.png)

Looking through that help display we can see the various key combinations that will perform an action. In this scenario we want to save and exit, so `Ctrl` + `KX` should be pressed.

**NOTE:** The `^` character signifies the `Ctrl` key.

**NOTE:** To hide the Help Screen press `Ctrl` + `KH` again.

Now display the contents of `file.txt` with the `cat` command to make sure our changes took place.

```text
~% cat file.txt
hi, I am on line 1 line 2 3rd is best
```

**Success!**

Open `file.txt` again and remove the third line. To do this first position cursor on line 3 and then press `Ctrl` + `Y`. For the sake of argument let's pretend you subsequently realized you needed line 3. Never fear, you can exit without saving by selecting `Ctrl` + `C`.

Go ahead and exit without saving changes.

**NOTE:** `joe` is great for times where you want to scroll up and and down in a large file. This scenario is also a good time to use `Ctrl` + `C` because even if you accidentally made changes you don't want to keep them because you were only using `joe` to more easily navigate the file. An alternative to displaying a file is to use the `cat`, `head`, or `tail` commands.

## Please proceed to the next step.

