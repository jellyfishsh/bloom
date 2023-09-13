This is an easy level challenge that I started out with a loooong time ago. So easy, in fact, that it would be a waste to do a writeup on it, as it takes little to no effort. 

Yet here we are. So why?

This is more of an experiment with making comprehensive writeups, so the format may change for this whole wargame challenge set until an acceptable format reveals itself to me.

**Note: I really, REALLY do suggest you try and go through this yourself. Its extremely easy and is really designed as a first-time learner's way to gather information and look things up. **
___

# Intro

Level 0 of the Bandit wargame is a setup to doing all of the other challenges, and is the "barrier of entry" for all the other wargames on this site.

Because of this, the bar is set low, as the only challenge is understanding how to use the terminal to connect to another computer across the internet.

This writeup assumes you have an operable Linux system in some shape or form.
# Connecting
This challenge wants the use of SSH in order to access the remote system.

SSH (or Secure Shell) is a command that allows you to remotely log onto another computer over the internet using TCP. It encrypts the traffic between the two computers, hence the secure.

The SSH command, written as just `ssh`, generally requires an host address and a username, written in the format:

`ssh <username>@<IP address>`

SSH has the default port of 22, so in base cases, a port does not need to be specified. However, this challenge requires you to use port 2220. So we must define to the command what port to use.

## Using man
You can use the wikiHow link that tells you what the keyword is for specifying a port. However, you can also read the manual page of this command to see all the options that you have for this command:

`man ssh`

In the Description section, there is a list of helpful keywords, or flags, to specify a certain value in the command. Reading through this list shows the entry for port.

`-p port: Port to connect to on the remote host. This can be specified on a per-host basis in the configuration file.`

With this information, we can write out our full command. Using the provided username, password, host address, and port, we can write the command:

`ssh <username>@<host address> -p <port number>`

Since its (probably) the first time the local host (us) has logged onto the remote host (the challenge), we need to accept the authenticity check.

After we do that, we are asked for a password. Entering the password, we can finally access the remote host, and complete the pre-challenge level 0.

*End.*