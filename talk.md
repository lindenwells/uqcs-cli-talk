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
    - `ssh s1234567@moss.labs.eait.uq.edu.au`
    - It will ask
