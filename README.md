# Local Dotfiles

These files are my .local modifications that I build on top of [thoughtbot/dotfiles](https://github.com/creativesoapbox/dotfiles) as the foundation of my personal configuration.

## Install

Install [thoughtbot/laptop](https://github.com/thoughtbot/laptop). Then install Thoughtbot's dotfiles:

```bash
git clone https://github.com/creativesoapbox/dotfiles
env RCRC=$HOME/dotfiles/rcrc rcup
```

Then clone mine if you dare:
```bash
git clone https://github.com/justinkuntz/dotfiles-local  ~/dotfiles-local
```

And re-run rcup to link:
```bash
rcup
```

## What's in it?

[vim](http://www.vim.org/) configuration:

* custom configuration broken down by subject area in vim folder
* rainbow parentheses to change colors of (), {}, [], <> when editing code
* vim-vinegar for quick jumps through the file system (use `-` to jump to
  folder view for current file)
* vim-haml & vim-markdown for editing those file/template types
* Other awesome @tpope plugins: vim-abolish, vim-dispatch, vim-repeat,
  vim-unimpaired.
* vim-blockle for toggling between Ruby do-end and {} block styles
* vim-textobj-rubyblock for getting Ruby method and class text objects (thanks
  to @nelstrom)
* vim-scratch for top-down visor-like scratchpad

[tmux](http://robots.thoughtbot.com/a-tmux-crash-course)
configuration:

* @christoomey's vim-tmux-navigator to streamline jumps between vim and tmux
  splits using the same commands at all times

[git](http://git-scm.com/) configuration:

* Use the Github shell command `hub` instead of `git` (backwards compatible with
  `git`)
* Pretty logging (courtesy of @croaky)

Shell aliases and scripts:

* `v` for neovim
* `rc` for rails console
* `taild` to tail development log
* `tailt` to tail test log
* `bex` for bundle exec
* `bu` for bundle update
* `heroky` for heroku, since I can't seem to spell that correctly when typing fast

Terminal stuff:
* nocorrects on parity commands: development, staging, production

## Credits

My configuration comprises of small changes on top of thoughtbot's dotfiles.
Also borrowed heavily from multiple sources:

[christoomey](https://github.com/christoomey), [thoughtbot/laptop](https://github.com/thoughtbot/laptop), [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles)

Thoughtbot has a great series of blog posts about dotfile configuration at their
[blog](http://robots.thoughtbot.com).


This software is free and distributable under the MIT license.
