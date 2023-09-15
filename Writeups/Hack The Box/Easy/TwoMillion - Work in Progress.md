# This Writeup is not complete!
My first writeup on the Hack the Box platform is interesting... because I have little to no experience. How would I, someone with almost no experience, have the gall to make a writeup??

Simple. I just learn from someone else and reinterpret it in my own words. Thats not to say that I'll do the entire thing from another writeup, but rather use my limited knowledge to create a writeup, find any knowledge gaps, and then explain that knowledge in a different way. I'll sum this up for every writeup that I do in a few simple words:

I would rather win by falling first.

So, lets get started with what I know!

# Enumeration
The address for my box is `10.10.11.221` . We can check any open ports and services by using the following command:

`nmap -sC -sV -Pn 10.10.11.221`

For context:
* `-sc` runs the default nse scripts for nmap, which do a plethora of things, like detecting vulnerabilities and checking for default settings on certain services
* `-sV` enables service detection, which lists informaiton about the services running on the ports specified.
* `-Pn` skips the ping sweep, which is used for host discovery.

quick test

