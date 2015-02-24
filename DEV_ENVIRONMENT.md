# Setting up a Development Environment

All of the code here can be run on any environment that has Ruby and Bundler installed. However, there can be small differences between environments. As such, we have made a Virtual Machine (VM) for trainees to utilize locally. To

**You will need to be connected to the internet to setup your environment, and depending on your connection speed it could take some time. Please do this in advance of attending the class!**

## Using Mac OS X locally

If you have already used Sass / Compass, and want to continue to do so, you may use you local Mac. This is how we generally develop our code, but occasionally minor differences between environments can cause errors. If you use your local machine, please ensure you have the following installed:

* Ruby (Version 2.0.0-p451 or higher)
* [Node.js](http://nodejs.org/download/) (Most recent)
* [Bundler](http://bundler.io/) (Installed via command line)
* [Yeoman](http://yeoman.io/) (npm install -g yo)

## Windows

These directions are meant for OS X and Linux hosts. Although the Vagrant machine should work on Windows, it have not tested it thoroughly. Taylor, one of the trainers, has successfully run this virtual machine on his Windows 8.1 machine, but cannot guarantee support on Windows.

## Prerequisites

This VM is built using [Vagrant](https://www.vagrantup.com/) and [VirtualBox](https://www.virtualbox.org/). You will need to download them both to proceed.

1. Download Vagrant: https://www.vagrantup.com/downloads.html
2. Download VirtualBox: https://www.virtualbox.org/wiki/Downloads

Each installation should be just as easy as click to install, but if you need more information, check out the documentation online.

1. Vagrant Documentation: https://docs.vagrantup.com/v2/installation/
2. VirtualBox Documentation: https://www.virtualbox.org/manual/ch02.html

## Download this class's repository

All of the source code for this training lives on GitHub. You can look at it all by going to https://github.com/tsmith512/arwd. If you are comfortable with the command line and use git, go to the directory you want to download the source code into, and run this command:

```bash
$ git clone git@github.com:tsmith512/arwd.git
```

If you are not confortable with the command line, please install [GitHub for Windows](https://windows.github.com/) or [GitHub for Mac](https://windows.github.com/). Both of these programs will give you a GUI to clone repositories with. [SourceTree](http://sourcetreeapp.com/) is also a great Git GUI for both platforms.

You may also download a ZIP of the whole project now, but you will need to download it again if it is updated: https://github.com/tsmith512/arwd/archive/gh-pages.zip

## Start up the development environment on Mac OS X

* Thanks to our amazing pals at [Amazee Labs](http://amazeelabs.com/), we have including some scripts to help setup the VM.
* Double click on vagrant-up.command to run the shell script for your OS. Important: On some OS X Installations you need right
click on the file and click "open".
* You will be prompted for a Password. Enter your system password and confirm with return
* After a couple of minutes (depending on your internet connection), you should see:

```bash
-------------------------------------
| Vagrant Booted Up                 |
-------------------------------------
| Visit this page to continue:      |
| http://192.168.111.42             |
-------------------------------------

logout

```

This will take time! Also, lots of information show up on the screen. We are downloading and setting up an entire linux server, so please do this in advance of the course.

If everything worked correctly, then you should be able to see a website at http://192.168.111.42/. Let us know if you have any questions or concerns.

## Start up the development environment on Windows 7/8

* Once you have cloned or downloaded the project repo, edit the `Vagrantfile`
* On line ~13 that starts with `config.vm.synced_folder...`
  * Remove `:nfs => true` at the end
  * Add `:mount_options => ["dmode=777,fmode=666"]` at the end instead

_Windows doesn't support NFS (although VirtualBox would just ignore that directive), so remove that. The `mount_options` directive instructs Vagrant to mount the shared folder with world-writable permissions, which will allow the Vagrant user to write to these files. The default permissions without NFS are read-only, but we need Sass to be able to generate its output. This is the only host-environment stumbling I ran into with Windows._

**Note:** The default shared folder behavior doesn't automatically update files in a way that Ruby can detect. You cannot run `bundle exec compass watch`, you must instead run `bundle exec compass compile` anytime you change the Sass files.

* From the command prompt, change directories into the project folder
* Run `vagrant up`
* From there, the machine will provision. Mac users see more frequent output to the console from Terminal than is provided by the Command Prompt, but it should be running fine. (If you're really curious, watch network utilization in `taskmgr`/`resmon`.)

Be sure to use `vagrant up` and `vagrant halt` from the command-line instead of using the VirtualBox UI.

## Recommended Editing Tools

To edit the files, you only need a text editor. (Don't use a word processor!) There are tools designed for it that will be more satisfying than a text editor.

Good tools for editing include [Coda](https://panic.com/coda/), [Notepad++](http://notepad-plus-plus.org/), [Sublime](http://www.sublimetext.com/), and [Atom](https://atom.io/). 
