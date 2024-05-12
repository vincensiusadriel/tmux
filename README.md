# tmux
a tmux config with tmux sessionizer from https://github.com/ThePrimeagen/.dotfiles

requires tmux
```
brew install tmux
```

requires fzf
```
brew install fzf
```

to clone it 

```
cd
git clone git@github.com:vincensiusadriel/tmux.git
ln -s -f tmux/tmux-sessionizer
ln -s -f tmux/.tmux.conf
```

add this line to your zshenv for sessionizer key bindings
```
bindkey -s ^f "~/tmux-sessionizer\n"
```

## For Ubuntu
add this to .bashenv / .bashrc
```
# Define a function to execute the desired command
tmux_sessionizer() {
    ~/tmux-sessionizer
}

# Bind the function to the desired key combination
bind '"\C-f":"tmux_sessionizer\n"'
```
