# ubuntu-migration
Tools for migrating to the next Ubuntu release vs upgrading. This is a WIP created as a result of Aptik being removed as an open source software to paid and proprietary. I have opted to not pay and discontinue use of the software as I feel that as a user of FOSS software, the code I write in turn should belong to the community. If I write code and expect others to pay for it, then I should be paying everyone who wrote the code in the software I am using. Since I am not a full developer and cannot contribute full pieces of software, I do share the scripts, settings, configurations and procedures that I use to make my life easier.

My intent is to address the issues of migration, all that Aptik addresses plus some of my own additions, and provide instruction and some bash script to allow users to perform successful migrations without relying on paid software. The needed functionality should be fairly easily accomplished with true open source software and/or some custom scripts.

## Areas to be addressed
1. Respositories and associated priority assignment
1. APT and DEB packages installed
1. Snap packages installed
1. Flatpak packages installed
1. Mounts
1. User accounts and groups
1. $HOME data
1. Dconf, which is in `$HOME`
1. Program data and settings from `/etc`
1. CRON / scheduled tasks
1. Icon, theme and font
1. Python (pip) and NodeJS (npm)
1. User scripts

## The repository
The respository will contain a collection of scripts to perform the above tasks for migration. Over time, I hope this to become a semi-automated set of scripts to make for easy migrations.

## Problems / Issues / Considerations
- Transferring settings can sometimes cause issues when newer versions of software are in the ugrade. Settings for prior versions of software _can_ cause issues in the associated programs.
- Programs, like Aptik, that automate this process can sometimes be unreliable. For example, the new version of Aptik is **NOT** compatible with backups performed with the prior free versions. The solutions outlined here can solve this by allowing you to keep control of the process.
- When upgrading Ubuntu, it is common that some of your installed softwares will be removed. This is one reason I prefer migration over upgrade. When I have a list of the softwares I have, I can choose which I want to keep ... and install any additional required packages needed at that time.
