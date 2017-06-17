# vim

## download this project content to home root dir (override existing .vim* will automatically enable exvim

## first time to create README.md file using command below
echo "# vim" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/skivvyxu/vim.git
git push -u origin master

## end

# ExVim Simple Way to install 
- step1 mkdir ~/exvim
- step2 cd ~/exvim and download exvim full pkg (http://exvim.github.io/docs/install/)
- step3 unzip the pkg inside ~/exvim

---
## Option 1 (Recommend): Source exVim to your current Vim

- step4 add content below into ~/.vimrc file

> let g:exvim_custom_path='~/exvim/'

> source ~/exvim/.vimrc

###### Now you can running exVim directly.
---

## Option 2: Replace your current Vim
- step4 To replace your current Vim to exVim, you can run the following scripts:

 for mac user 

> sh osx/replace-my-vim.sh

 for linux user
> sh unix/replace-my-vim.sh

If you are Windows user, you can run this batch script in command line window:

The commands above will do three things:

1. replace your ~/.vimrc with exVim's .vimrc.
2. copy .vimrc.plugins to ~/.vimrc.plugins.
3. copy and rename vimfiles/ to ~/.vim/.

**NOTE**: In Windows, the exVim's .vimrc also rewrite the runtimepath settings to make it search ~/.vim folder instead of ~/vimfiles
