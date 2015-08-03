<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Main task: finish the evil-tutor</a></li>
<li><a href="#sec-2">2. Bonus tasks: more vim</a>
<ul>
<li><a href="#sec-2-1">2.1. Simple macros</a>
<ul>
<li><a href="#sec-2-1-1">2.1.1. Infos</a></li>
<li><a href="#sec-2-1-2">2.1.2. Exercise</a></li>
</ul>
</li>
<li><a href="#sec-2-2">2.2. More vim power</a>
<ul>
<li><a href="#sec-2-2-1">2.2.1. Infos:</a></li>
<li><a href="#sec-2-2-2">2.2.2. Exercise</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</div>
</div>


# Main task: finish the evil-tutor<a id="sec-1" name="sec-1"></a>

The task for this day is easy: **finish the evil-tutor**. Just use M-x to bring up the command console and enter **evil-tutor-start**

# Bonus tasks: more vim<a id="sec-2" name="sec-2"></a>

## Simple macros<a id="sec-2-1" name="sec-2-1"></a>

### Infos<a id="sec-2-1-1" name="sec-2-1-1"></a>

A basic feature of every serious text editor are macros. To keep it easy, we'll just use the Emacs quick-fix macros. This should get you going:

To define a macro and run it:

1.  Press F3. The bottom line will now say: "Defining keyboard macro"
2.  Do whatever you want to do, ideally choose a workflow that combines an editing operation and a movement operation (solve the task below for an example)
3.  Press F4. The minibuffer (bottom line) now shows: "Keyboard macro defined"
4.  Pressing F4 again will apply the macro at the current caret position! Awesome!

### Exercise<a id="sec-2-1-2" name="sec-2-1-2"></a>

The following text needs to be converted into a list, and the first word in each line should be bold. So,

**Get this text:**

    Formatting text with
    macros is incredibly useful,
    particularly when I copy and paste text
    from the internet, for example
    code or stuff from
    documentations

**To look like this:**

-   **Formatting** text with
-   **macros** is incredibly useful,
-   **particularly** when I copy and paste text
-   **from** the internet, for example
-   **code** or stuff from
-   **documentations**

**By applying a simple macro to all lines**

*Tips:*
-For now, use Esc to switch between insert and normal mode, not keychords such as *fd* while recording macros

-   just do this in the first line and record it as a macro which can then be applied to the other lines: 
    -   Go to the beginning of the line and insert "- \*" in front of the first word
    -   Go to the end of the first word and insert "\*"
    -   Move down one line

## More vim power<a id="sec-2-2" name="sec-2-2"></a>

### Infos:<a id="sec-2-2-1" name="sec-2-2-1"></a>

Look into these commands to get a taste of what is till waiting for you. This should be very easy to google so I don't bother explaining it here.

    :normal
    :g//

### Exercise<a id="sec-2-2-2" name="sec-2-2-2"></a>

**Get this**

    file1.txt
    file2.txt
    file3.txt

**To look like this**

    ~/project/path/to/file/file1.txt
    ~/project/path/to/file/file2.txt
    ~/project/path/to/file/file3.txt

**Using only one *:normal* command**

*Tips:* 

-   To paste in the minibuffer, use *Ctrl-Y* for now. We will come to better ways for handling complex commands and dealing with your command history later.
-   Use visual line mode (press V and j to mark the lines) before applying :normal, then you will automatically have the correct range!