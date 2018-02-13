# Neovim for Nokia N900

![alt text](https://talk.maemo.org/attachment.php?attachmentid=39752&stc=1&d=1518508056)

These are just repacked Debian Stretch installers (since building Neovim for the n900 always failed for me); installing them are working fine.

WARNING! Neovim depends on libc6 >= 2.7 but Maemo5 has only 2.5.1. So I built 2.10 on the device based on this idea: http://talk.maemo.org/showthread.php?t=89467. I have been using it for a week now on my main every-day-used n900 and I didn't experience any issues so far (hmm... only one thing: BlessN900 freezes when taking HDR photos). BUT I MUST WARN YOU THAT INSTALLING THIS VERSION OF LIBC6 CAN BRAKE MAEMO5 INSTALLATION SO YOU ARE RISKING A REFLASH.
I installed only libc6_2.10 and locales_2.10.

XSEL is needed to be able to use clipboard in neovim. This version is from here: https://talk.maemo.org/showpost.php?p=1234420&postcount=6


After installing the debs you need to create ~/.config/nvim folder and init.vim file in this folder - i.e. init.vim is like vimrc and the content can be the same. Some of the plugins (for example csv.vim, vim-airline) should go in ~/.config/nvim/plugged folder.
