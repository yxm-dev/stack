The following is a list of softwares and settings I have been used in the last years. The marked items are
those that I'm currently using.

In very few words, I use:

- [Arch Linux](https://archlinux.org/), as my linux distribution
- [i3](https://i3wm.org/), as my windows manager
- [xterm](https://invisible-island.net/xterm/) as my terminal emulator.

I try to do everything is possible inside terminal. If something cannot be embedded in a terminal I embed it in
a browser. For that I use:

- [firefox](https://www.mozilla.org/pt-BR/firefox/new/), for diary stuff
- [tor](https://www.torproject.org/), when privacy is needed.

My text editor is `vim`. I use `mutt` as my mail client.
       
Linux Distribution
-----------------

* [Arch Linux](https://archlinux.org/) (*)
    * [base](https://archlinux.org/packages/core/any/base/) (*): package with basic libraries and utilities.
      Among them one has:
        * [bash](https://archlinux.org/packages/core/x86_64/bash/): the default shell in Arch. By `GNU`  
        * [file](https://archlinux.org/packages/core/x86_64/file/): file type identification tool.
        * [filesystem](https://archlinux.org/packages/core/x86_64/filesystem/): the default file structure for
          Arch.
        * [gawk](https://www.gnu.org/software/gawk/manual/gawk.html): `GNU` implementation of the `awk`
          programming language
        * [linux](https://archlinux.org/packages/core/x86_64/linux/) (optional): Linux kernel headers and development files
        * [linux-firmware](https://archlinux.org/packages/core/any/linux-firmware/) (optional):
        * [pacman](https://archlinux.org/packages/core/x86_64/pacman/): package manager for Arch
        * [sed](https://archlinux.org/packages/core/x86_64/sed/): command line text editor. By `GNU`
        * [systemd](https://archlinux.org/packages/core/x86_64/systemd/): init system used by default in Arch
        * [tar](https://archlinux.org/packages/core/x86_64/tar/): manage `.tar.gz`  files
        * [xz](https://archlinux.org/packages/core/x86_64/xz/): manage `.xz` files
    * [base-devel](https://archlinux.org/packages/core/any/base-devel/) (*): package with basic tools and
      libraries for development. Among them:
        * [autoconfig](https://archlinux.org/packages/core/any/autoconf/): automatically configuring source
          code. By `GNU`.
        * [automake](https://archlinux.org/packages/core/any/automake): automatically creating makefiles. By
          `GNU`
        * [gcc](https://archlinux.org/packages/core/x86_64/gcc/): `GNU` collection of compilers and tools for
          `C`-based languages
        * [make](https://archlinux.org/packages/core/x86_64/make/): automation build tool. By `GNU`.
        * [sudo](https://archlinux.org/packages/core/x86_64/sudo/): allow normal users act as root users.
        * [which](https://archlinux.org/packages/core/x86_64/which/): show the full path of commands.
    
Windows System
----------------

* [x11](https://www.x.org/wiki/) (*)

Windows Manager
-----------------

* [openbox](http://openbox.org/wiki/Main_Page): stacking windows manager 
* [i3](https://i3wm.org/): tiling windows manager (*)

UI/UX
---------

* [ncurses](https://www.gnu.org/software/guile-ncurses/)

Terminal Emulator
--------------------

* `Lxterminal`
* [xterm](https://invisible-island.net/xterm/) (*)

* **Remark**: I use `Liberation Mono` font. In Arch it is in the package `ttf-liberation`. 

Driver Managers
----------------

* ALSA driver [sound] (*)
    * `amixer` + `alsamixer`: builtin CLI and TUI managers for ALSA. (*)
    * `pulseaudio`: daemon for multiplex sound stuff (*)
        * `pulseadio-alsa`: package to allow pulseaudio to control ALSA (*)
        * `pavucontrol`: GUI for pulseaudio
    
* INTEL driver [video] (*)
    * `xrandr`: a daemon for INTEL driver (*)
    * `lxrandr`: GUI for `xrandr`
     
* `networkmanager` [wireless] (*)
    * `nmcli` + `nmtui`: CLI and TUI interfaces for `networkmanager`. (*)

Compilers/Interpreters
------------------------

* `bash`: default shell for the `Linux` kernel (*)
    * contained in the base Arch package 
        
* `Texlive` (*):
    * with ... for:
        * ...
        
* `Python` (*)
    * `python-pip`: package manager for `python` (*)
        - `khard`: address manager. Use with `mutt`) (*)
        - [pandoc_static_katex](https://github.com/Zaharid/pandoc_static_katex): for `sw.sh` (*)
        - [urlscan](https://github.com/firecat53/urlscan): url manager. Use with `mutt` (*)
        - [socli](https://github.com/gautamkrishnar/socli): CLI for Stack Overflow (*)
        - [aws-cli](https://github.com/aws/aws-cli): CLI for AWS (*)

* `Haskell` (*)
    - `pandoc` (markup languages converter) (*)

* `pandoc`: command line markup languages translator. (*)
    * used in `cvt.sh`
    * see below
        
* `Ruby`
    * `rubygems`: package manager for `Ruby`
        - `Jekyll`
        
* `Go`
    * `spotify-tui`
    
* `Node.js` (*)
    * `npm`: package manager for `Node.js`. (*)
        - `dicio`: [link](npm install --global dicio)
        - `gramma`: [link](https://github.com/caderek/gramma)
        - `katex` (for `pandoc_static_katex`):

Building
--------

* [make](https://www.gnu.org/software/make/) (*): UNIX build automation tool. By `GNU`
    * contained in Arch's [base-devel](https://archlinux.org/packages/core/any/base-devel/) package.
* [autoconfig](https://www.gnu.org/software/autoconf/) (*): automatically configuring source code. Used with make. By `GNU`.
    * contained in Arch's [base-devel](https://archlinux.org/packages/core/any/base-devel/) package.
* [automake](https://www.gnu.org/software/automake/) (*): automatically creating makefiles. By `GNU`
    * contained in Arch's [base-devel](https://archlinux.org/packages/core/any/base-devel/) package.
* [cmake](https://cmake.org/): platform independent build generator.


File Handing
--------------

* [grep](https://www.gnu.org/software/grep/) (*): search in files. By `GNU`.
    * contained in Arch's [base](https://archlinux.org/packages/core/any/base/) package
* [rsync](https://github.com/WayneD/rsync) (*): command line tool to sync files locally and remotely
    * used in  [sync.sh](https://github.com/yxm-dev/sync.sh) and in [gp.sh](https://github.com/yxm-dev/gp.sh)
* [rclone](https://rclone.org/) (*): command line to sync files with/between clouds
    * used in [bkp.sh](https://github.com/yxm-dev/bkp.sh)
* [tar](https://www.gnu.org/software/tar/) (*): manage `.tar.gz` files. By `GNU`
     * contained in Arch's [base](https://archlinux.org/packages/core/any/base/) package 
* [zip](https://infozip.sourceforge.net/Zip.html) + [unzip](https://infozip.sourceforge.net/UnZip.html) (*): manage `.zip` files
           
Text
------

* [sed](https://www.gnu.org/software/sed/) (*): command line text editor. By `GNU` (*).
* `nano`: text-based text editor. By `GNU`.
    * used only to install Arch. 
* `vim` (*): TUI extendable text editor.
    * `vimwiki` (*)
        * `vimwiki-cli`: [link](https://github.com/sstallion/vimwiki-cli)
        * `vim-Calendar`
    * `vimtex` (*)
        * `vimtex-Colors` (*)
    * `fzf-bibtex`: bibtex manager based on `fzf` - [link](https://github.com/msprev/fzf-bibtex)
    * `vim-snippets`
    * [delimitmate](https://github.com/raimondi/delimitmate): automatically close brackets, etc.
* `zathura`: simple `pdf` reader. (*)
    - `zathura-djvu`: add compatibility with `djvu` files (*)
    - `zathura-pdf-mu-pdf`: add some features and compatibility with `epub` files (*)


Web
----

* browsers
    * `w3m`: text-based browser (*)
    * [firefox](https://www.mozilla.org/pt-BR/firefox/new/): open-source browser (*)
    * [tor](https://www.torproject.org/): privacy-based browser (*)
        
* mail
    * `mutt`: text-based email client (*)
        - [urlscan](https://github.com/firecat53/urlscan) : url manager (*)
    * [abook](https://github.com/hhirsch/abook): address manager  
    * `khard`: address manager (*)
    
* tools
    * [wget](https://www.gnu.org/software/wget/)
        * contained in    


Media
--------

* [imagemagick](https://imagemagick.org/index.php): command line image manipulation and conversion. (*)
    * used in the `lock.sh` script
* [scrot](https://github.com/resurrecting-open-source-projects/scrot): command line screenshot tool
* [imgur.sh](https://github.com/tremby/imgur.sh): `bash` script to upload images to
  [Imgur](https://imgur.com/) from command line.
* `ffmpeg`: command line video manipulation and conversion (*)
    * used in `cvt.sh`
* `sox`: command line audio converter (*)
    * used in `cvt.sh` 
* `spotifyd`: daemon for Spotify
* `spotify-tui`: terminal-based user interface for Spotify

DevOps Tools
---------

* [bc](https://www.gnu.org/software/bc/) (*): command line calculator. By `GNU`.
* `xsel`: command line [x11](https://www.x.org/wiki/) selection and clipboard manipulation tool (*)
    * used with `w3m` to copy to clipboard the url under cursor
* `fzf`: terminal-based fuzzy finder tool. (*)
    * used in `pm.sh`
* [git](https://git-scm.com/): version control system (*)
    * [github-cli](https://github.com/cli/cli): command line client for Github  (*)
    * [tig](https://github.com/jonas/tig)
* `docker`: containerization application (*)


Other
-------

* `translate-shell`: terminal-based interface for google translator - [link](https://github.com/soimort/translate-shell)
    * `trsl.sh`: simple interactive mode for `translate-shell`
* `dicio`: CLI for [dicio.com.br](https://www.dicio.com.br/), a Portuguese dictionary - [link](npm install --global dicio)
* `grammar`: CLI grammar checker based on [LanguageTool](https://languagetool.org/) - [link](https://github.com/caderek/gramma)

