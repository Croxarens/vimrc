This guy ![Ruchee](https://github.com/ruchee) did an awesome work with all the settings and plugins for VIM. I just forked his repo and edited what I needed for my setups.

I also added some other plugin :
 * vim-gitgutter
 * vim-fugitive

I use [powerline](https://github.com/powerline/powerline/tree/master), so you'll also find some settings related to it.

---
### Screenshot
![Vim Ruchee](https://raw.github.com/Croxarens/vimrc/master/macvim.jpg "Vim Ruchee")

----

#### Linux - Installation

1. For Debian/Ubuntu `sudo apt-get install vim-gtk exuberant-ctags git` [Check the equivalent packets names if you use another Linux distro]
2. Delete the .vim folder and the .vimrc file (if any) in the personal home directory : `rm -rf ~ / .vim ~ / .vimrc`
3. Use git to download the repo, then copy the subdirectory of the project in the personal home directory, and rename __vimfiles__ to __.vim__, and __\_vimrc__ to __.vimrc__ : `mv ~/vimrc/vimfiles ~/.vim && mv ~/vimrc/_vimrc ~/.vimrc`
4. You can download the __Monaco__ font from https://github.com/todylu/monaco.ttf/blob/master/monaco.ttf?raw=true . Use the command `mv monaco.ttf ~/.fonts/.` to drop it into .fonts folder.

----

### Precautions

 1. If the shortcut keys do not respond to the situation, please check whether you have opened other software (such as Kingsoft, etc.), some software shortcuts and Vim may conflict, simply modify or disable the software shortcut keys.
 2. This configuration defaults to the relative row number. If you are not used to comment, you can comment out the set relativenumber in the configuration to use the absolute line number.
 3. If conditions permit, it is best to use universal-ctags instead of the old ctags.
 4. Some plugins require scripting language support, and if conditions permit, please install Lua, PHP, Python, Ruby, Node, TypeScript and other language operating environment
 5. Please try to use the latest version of Vim 8.x, the lower part of the function may not be used.

----

### Simple CTAGS - Instructions

 1. First make sure that the system can find _ctags_, and that ctags is added to the system's path environment variable.
 2. While you are editing a souce file, type a small number of characters of some function and then press _Ctrl + P_ to have a simple code completion.
 3. Move the cursor to the function name you want and press enter.
 4. Press _Ctrl +]_ and VIM will automatically jump to the definition of the function.
 5. Press _Ctrl + T_ to return to the location before the jump.

More than just ctags simple usage, more professional introduction please Google, and another more powerful weapon YouCompleteMe so you explore (this configuration does not integrate the plug-in, please install it)
