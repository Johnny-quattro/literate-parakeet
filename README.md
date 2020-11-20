# literate-parakeet
This is a rather boring text file detailing nothing in particular. This repo will be added to and embellished in the near future.
I intend to use this repo for Raspberry Pi projects, namely Pi4 and Pi400.

=====================================================================================

The script 'ssh_monitor' was built over a period of time, after encountering many brute-force attacks on my Linux/Unix machines.
In fact, the greatest impetus came directly from my HP C360 workstation running HP-UX, which was being attacked relentlessly.

I understand that most automated attacks just try to hit port 22 but some are more devious.
I would certainly recommended changing the default port of 22 to something different.
Script variant created solely for use on Raspberry Pi due to differing syslog format compared to Devuan

Devuan-specific script: ssh_monitor

Raspberry Pi-specific script: ssh_monitor_pi

Recommended Usage: Run as a cron task every minute, although it can always be run manually from the shell prompt.

Requires: file /root/ssh-scan-blocked-table (dealt with in script logic)
