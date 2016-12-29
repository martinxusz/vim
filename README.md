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
- step4 add content below into ~/.vimrc file

---
> let g:exvim_custom_path='~/exvim/'
> source ~/exvim/.vimrc
---
