My dotfiles.

## .zshrc

```shell
export DOTFILES=$HOME/.dotfiles
export PATH="$DOTFILES/bin:$PATH"

for topic_folder ($DOTFILES/*) if [ -d $topic_folder ]; then  fpath=($topic_folder $fpath); fi;
autoload -U $DOTFILES/functions/*(:t)
```
