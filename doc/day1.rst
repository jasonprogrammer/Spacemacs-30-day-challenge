Day 1 - vim skill level: Stormtropper
=====================================

    :Author: Stephen Kraemer

.. contents::


1 Before we get started: install Emacs and Spacemacs
----------------------------------------------------

Spacemacs is officially compatible with Emacs 24.3 and 24.4. Personally,
I have had good experience with Emacs 24.5.

1.1 Getting a recent Emacs version in Linux
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you want a more recent Emacs version than your package manager
provides (e.g. because your Admin still has you on an old SUSE version)

- Ubuntu/Kubuntu:

  - Add the ppa:ubuntu-elisp/ppa to obtain new versions of Emacs
    (`https://launchpad.net/~ubuntu-elisp/+archive/ubuntu/ppa <https://launchpad.net/~ubuntu-elisp/+archive/ubuntu/ppa>`_)

- Suse

  - **Do not** install recent Emacs version from tumbleweed or factory
    repos if you are not on those releases!

  - Go to software.opensuse.org

  - search for emacs

  - go to the unstable packages

  - find the editors ppa

  - Install from there with 1 Click install

1.2 Getting a recent emacs version on Mac
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`https://github.com/syl20bnr/spacemacs#os-x <https://github.com/syl20bnr/spacemacs#os-x>`_

1.3 Getting spacemacs
~~~~~~~~~~~~~~~~~~~~~

`https://github.com/syl20bnr/spacemacs#install <https://github.com/syl20bnr/spacemacs#install>`_

2 First steps with vim
----------------------

2.1 Why you should take the time to learn vim
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**It really doesn't take that long. After 2h you should be faster than you were in those dark ages BV (before vim)**

I. **Vim is very ergonomic and fast**

- With vim key bindings, you have your hands on the home row at all
  times - I like that much better that having to reach for Ctrl and
  Alt all the time. There is a reason why there have always been vim
  ports to Emacs and other text editors.

- No one has had to use the Esc key in vim for 30 years. You can
  quickly press jj, jk, fd etc. instead of Esc to switch modes

- Btw., I have switched my Escape and Caps Lock keys anyway, because
  even without needing Escape in vim this is just practical

II. **Vim is a widely supported, much-loved standard for key bindings: if you know vim, you can rely on your muscle memory almost everywhere!**
   Programs which support vim key bindings

- Other text editors

  - Sublime (works fine)

  - Kate (never tried it)

  - Dedicated vim editors

    - Terminal vim

    - Gvim

    - Emacs (that's right, Emacs is as much a vim editor as Gvim
      and any other implementations)

- Rstudio, IDEs etc.

  - Rstudio

  - PyCharm and all other IntelliJ platforms (these are the most
    popular IDEs for Java, python etc.)

- Wikis etc.

  - TiddlyWiki

- Browsers

  - Chrome

  - Firefox

- Any GNU readline based program, i.e.

  - your konsole/terminal

  - ipython

  - The R language shell

  - Note The default key bindings in your terminal, however, are
    Emacs

- Office programs

  - Libreoffice (works ok)

  - Many online publication tools, such as *authorea* and
    *overleaf* over it or will offer it in the browser.

III. **Vim is great fun - it will make you feel like one of those superhackers from a cliche Hollywood movie**
.. image:: ./../img/swordfish.png

*This could be you!*

2.2 Try it out with the vim tutorial
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once spacemacs is running, press **Alt-x**, go for **evil-tutor-start** and
have some fun!
