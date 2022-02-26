# Talk topics I want to cover

- ssh
  - eligibility for moss
  - ssh keys (link to something)
- purpose of this talk
  - wow you with these tools (vim, ssh, cli, tmux)
  - how to get started (install ssh and use moss or do locally)
  - how to learn vim (vimtutor)
  - show you some workflows (2310, quick python scripts etc)
  - In this world of IDEs and extensions, get you to consider CLI where applicable
- not the purpose of this talk

  - oh fr? that's wild my g but I don't feel like spending hours configuring stuff, ceebs so I'm using vscode.
  - that's so cool I'm gonna start sending emails on command line and wiping my Windows to go full Arch bro

- ssh

  - ssh is both a protocol for securely accessing the shell on a remote machine and the name of the program you use to invoke it. Overloading, yeah it happens a lot.

  - If you are a student of EAIT in the current semester, you have access to moss.
    What's moss? It's a UQ-run computer that students can "connect" to from anywhere with internet using ssh (secure shell)
  - https://student.eait.uq.edu.au/infrastructure/remote-access/ssh.html

    - [https://student.eait.uq.edu.au/labs/myaccess/](Where will your student card get you?)
    - [https://student.eait.uq.edu.au/accounts/chsh.ephp/](Change your shell)

  - I'm going to talk about different paths to a terminal with ssh installed. My goal once I've done that is to be able to type `ssh` into a terminal and get the usage info back.

  - Windows (probably most people?):

    - If you can access moss and you can rely on an internet connection, I recommend "ssh-ing into" moss for everything. If internet is iffy, I recommend WSL (Windows subsystem for Linux). I don't recommend dual-booting Linux unless you have a good reason to. It can be spain without the s (but hey if you wanna do it don't take my word for it)

    - get windows terminal from the microsoft store. I don't like being told to install software, but trust me it's the best first-party terminal for Windows that I know of.

    - Even if you don't, you'll use PowerShell to invoke the program `ssh`

    - ssh is installed by default since April 2018 update

    - PuTTY is an option but I see little reason to now as it takes more clicks to start and is way uglier (you do you but I dislike trying to make my terminal sexy, prefer something that looks good out-of-the-box)

  - Mac/Linux:

    - you will have `ssh` installed already.

  - At this point, type `ssh` into whatever terminal you're using and success is seeing `usage: ssh ...`

  - Connecting to moss:

    1. `ssh s1234567@moss.labs.eait.uq.edu.au`
    2. It will ask if you trust the fingerprint or something.
    3. Type in the same password you would use to log into my.uq.edu.au

  - vim

    - Why vim?

      - It's lightweight and probably more importantly, one of your few options in some cases. If you told me to edit a file on my UQ home drive (that's the one you can access by logging onto a lab PC) right now, I would ssh into moss and use vim to edit the file. If you're renting a virtual private server (VPS), then possibly the only way of working with files on it is with a terminal. If you need to edit a file and all you have is a terminal, you're gonna need a CLI editor.

    - A wowee vim demo such as [Neil's](https://youtu.be/TIS7zS-yN04?t=426)?

    - undo tree: tell a story

    - weird arrow keys hjkl

    - modes (WHY CAN'T I TYPE?!!1)

    - operators and motions

    - copying between files

    - plugins

      - vim-coc for Intellisense autocomplete.

        - provide a demo of explore a nested structure, like a deep JS object.

    - How to learn? vimtutor. vimtutor is the official way to learn vim. It just loads up a temp file that you can play around with. It will explain stuff so much better than I could, and since you're typing stuff out yourself, you will probably retain info better. It will take an hour or so
