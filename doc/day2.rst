Day 2: vim skill level: Padawan!
================================

    :Author: Stephen Kraemer

.. contents::


1 Finish the evil tutor
-----------------------

The first task for this day is simple: **finish the evil-tutor**. Just use M-x to bring up the command console and enter **evil-tutor-start**

2 Learn the power of macros
---------------------------

2.1 Infos
~~~~~~~~~

A basic feature of every serious text editor are macros. To keep it easy, we'll just use the Emacs quick-fix macros. This should get you going:

To define a macro and run it:

1. Press F3. The bottom line will now say: "Defining keyboard macro"

2. Do whatever you want to do, ideally choose a workflow that combines
   an editing operation and a movement operation (solve the task below
   for an example)

3. Press F4. The minibuffer (bottom line) now shows: "Keyboard macro
   defined"

4. Pressing F4 again will apply the macro at the current caret position!
   Awesome!

2.2 Exercise
~~~~~~~~~~~~

The following text needs to be converted into a list, and the first word
in each line should be bold. So,

**Get this text:**

.. code-block:: sh

    Formatting text with
    macros is incredibly useful,
    particularly when I copy and paste text
    from the internet, for example
    code or stuff from
    documentations

**To look like this:**

- **Formatting** text with

- **macros** is incredibly useful,

- **particularly** when I copy and paste text

- **from** the internet, for example

- **code** or stuff from

- **documentations**

**By applying a simple macro to all lines**

Tips:

- For now, use Esc to switch between insert and normal mode, not keychords such as *fd* while recording macros

- just do this in the first line and record it as a macro which can then be applied to the other lines:

  - Go to the beginning of the line and insert "- \*" in front of the
    first word

  - Go to the end of the first word and insert "\*"

  - Move down one line

3 Apply powerful line-based transformations to regions and whole documents
--------------------------------------------------------------------------

3.1 Infos:
~~~~~~~~~~

3.1.1 Ranges
^^^^^^^^^^^^

Many evil/vim commands can be used on user-defined regions. You have already met the substitution command **:s**, which is good example for this class of commands. If you want to have an impression of the full complexity, have a `look here <http://vim.wikia.com/wiki/Ranges>`_. 

For now, all you need to remember is

- Most commands will operate on the current line only by default

- if you make a visual selection and call a command afterwards, the command will be applied to the selected region.

Try it! Use the **:s** command to make a substitution in a couple of visually selected lines. When you press **:s** you will see **:'<,'>s** in the command line, indicating that the command will work on the whole selected region.

3.1.2 Commands for line-based editing of whole regions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Look into these commands to get a taste of what is till waiting for you. This should be very easy to google so I don't bother explaining it here.

.. code-block:: sh

    :normal
    :g//

3.2 Exercise
~~~~~~~~~~~~

**Get this**

.. code-block:: sh

    file1.txt
    file2.txt
    file3.txt

**To look like this**

.. code-block:: sh

    ~/project/path/to/file/file1.txt
    ~/project/path/to/file/file2.txt
    ~/project/path/to/file/file3.txt

**Using only one *:normal* command**

*Tips:*

- To paste in the minibuffer, use *Ctrl-Y* for now. We will come to better ways for handling complex commands and dealing with your command history later.

- Use visual line mode (press V and j to mark the lines) before applying :normal, then you will automatically have the correct range!
