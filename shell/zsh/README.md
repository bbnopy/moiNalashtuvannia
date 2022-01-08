# ZSH shell

perevirka *shell* yakyi vykorystovuietsia

```zsh
$ echo $SHELL
```

vstanovlennia *zsh-shell*

```zsh
$ sudo pacman -S zsh zsh-completions
```

zapuskaiemo *zsh*

```zsh
$ zsh
```
varianty vyboru 1, 2, 1, 0, teper vstanovliuiemo

```zsh
$ yay pacman -S oh-my-zsh-git
$ cp /usr/share/oh-my-zsh/zshrc ~/.zshrc
$ sudo pacman -S ruby
```

vstanovlennia *zsh* za zamovchenniam dlia pevnoho yuzera

```zsh
$ chsh -s /bin/zsh/username
```

vstanovlennia *zsh* dlia usih

```zsh
$ chsh -s(which zsh)
```