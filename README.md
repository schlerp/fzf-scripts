# fzf-scripts

This is a collection of fzf scripts for use in my terminal based workflow.
Specifically I use `tmux` and `nvim`.
You will find descriptions of the scripts along with suggestions for mappings in your tmux config where it makes sense to be bound to a key in `tmux`.

## Scripts

### ffg - Fuzzy File Grep

This script is pretty much straight from the fzf advanced documentation.
It is a nice way to search for files using rip grep and filtering with fuzzy searching provided by ripgrep.
I use it most of the time just to grep over files when I'm looking for examples of how something is used.
I can use fzf to find the files, then if there is something I need LSP features for (like jump to definition etc.) then I hit enter and use the LSP in neovim to jump around.

#### Features

* Uses `bat` to give a preview of the file/line you've matched
* pressing `return` will cause that file/line to be opened in `neovim`

#### Dependencies

* bat - `brew install bat`
* ripgrep - `brew install ripgrep`
* nvim - `brew install neovim`

#### Inspiration/Origins/Kudos

* [junegunn/fzf - ADVANCED.md](https://github.com/junegunn/fzf/blob/master/ADVANCED.md)
