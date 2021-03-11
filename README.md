<h1 align='center'>
vim-gitgrep
</h1>

<p align='center'>
Searches the project using <code>:GG &lt;search&gt;</code> and show it in a new buffer. Inspired by Sublime Text's Find in Files feature.
</p>

![Screencast](images/preview.gif)

## Install

Install using vim-plug:

```vim
Plug 'rstacruz/vim-gitgrep'
```

Search using `:GG`:

```
:GG hello
```

Read the [documentation](./doc/gitgrep.txt):

```vim
:help gitgrep
```

## Tips

This will bind <kbd>leader</kbd><kbd>g</kbd> to search the current word under the cursor, similar to pressing <kbd>\*</kbd>.

```vim
nnoremap <leader>*  :GG! <C-r><C-w><CR>
vnoremap <leader>*  y:GG! <C-r>"<C-b><CR>
```

This will bend <kbd>leader</kbd><kbd>/</kbd> to put `:GG! ` in the command line, ready to accept input.

```vim
nnoremap <leader>/  :GG!<space>
```

## Thanks

:heart: MIT
