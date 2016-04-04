Paroodise
=========
Paroodise is a scripted implementation of [this](http://unix.stackexchange.com/questions/226872/how-to-shrink-root-filesystem-without-booting-a-livecd/#answer-227318).

## Usage
SSH/Login with root, then:
```
 git-clone https://github.com/natostanco/paroodise
 cd paroodise
 nohup ./prd
```
Restart your shell and you should be inside root on tmpfs (RAM).
Reboot to restore normal operations.

## Notes
- The script has been mainly tested with Debian 8.

## Purpose
It was created to perform actions on the main storage device of virtual machines. Specifically to install less common OSes (CoreOS, RancherOS, PA) from common already available ones (Debian,CentOS, Ubuntu) with hosts who do not provide custom ISOs installations. This process is very fast and does not require do download any package or create fs images to then load from grub like in common boot to ram processes.


