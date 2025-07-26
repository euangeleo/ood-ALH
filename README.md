O'odham (Alvarez-Hale orthography) keyboard
==============

© emj

Description
-----------
This keyboard is designed to allow quick typing of O'odham data in the Alvarez-Hale writing system.

Supported Platforms
-------------------
 * all [desktop platforms](https://help.keyman.com/developer/language/reference/targets) (includes Windows and macOS, but only tested on Linux)
 
To compile on Linux
-------------------
Following instructions [here](https://community.software.sil.org/t/how-to-install-an-kmn-source-kmfl-file-onto-ubuntu-24-04/8864/5) (which seem to be the same as [here](https://help.keyman.com/knowledge-base/?id=114)) to compile a Keyman keyboard in Ubuntu linux without Keyman Developer.

* Install node.js 18.0 or later. (I an in Ubuntu 22.04, and the highest version of node.js in the repos is 12.0, so chose to [install from a PPA](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-22-04#option-2-installing-node-js-with-apt-using-a-nodesource-ppa).)
* Install Keyman keyboard compiler:

```terminal
sudo npm install -g @keymanapp/kmc
```

* Run compiler (from the root directory of this project): 
```terminal
 user@machine:~$ kmc build ood-ALH.kpj
```

* The .kmp file should now be in `build`. You can install it with the Keyman Configuration utility. There are instructions [here](https://help.keyman.com/products/linux/current-version/common/) to install Keyman for Linux in Ubuntu 22.04 or later. Once installed, you should find the Keyman Configuration utility in the app launcher.

