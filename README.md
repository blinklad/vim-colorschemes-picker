

## ABOUT ##

Power VIM Users like us have already wasted tons of time to choose our favorite colorschemes, and may still not be satisfied with the current colorschemes. *V*im*R*and*Colour* is not here to necessarily help you, it's here to add nondeterministic aesthetic into your daily life of editing text.

How does this work? How are colours selected?
__Who knows__, really. Some guesses, though...
1. When you start Vim;
2. When you open a buffer;
3. When you read or write to a buffer;
4. When you open a split;
5. Much, much more...


This plugin has been adapted in a slightly more opinionated fashion to suit the current authors preference for the [Base16 project](https://github.com/chriskempson/base16) as well as memes. 
Like real life, memes can be opted out of through the provided variables. 


### Installation ###


### Pathogen 
If you have pathogen installed and can just copy into ~/.vim/bundle like this:

```cd ~/.vim/bundle ```
``` git clone https://github.com/sunuslee/vim-plugin-random-colorscheme-picker ```

if you are using Janus:

``` cd ~/.janus && ```
```git clone https://github.com/sunuslee/vim-plugin-random-colorscheme-picker ```


### Vim-Plug

```plug 'blinklad/vim-rand-colour' ```

### [Bundle](https://github.com/gmarik/vundle)
```Bundle 'bkbncn/vim-colorschemes-picker'``


### Without Pathogen, Vim-Plug or Bundle###
Just copy randomColorPicker.vim to your VIM runtime plugin path:


##### Linux #####

You may need to create ~/.vim/plugin directory if it doesn't exist:

```mkdir -p ~/.vim/plugin```

then:

```cp plugin/randomColorPicker.vim ~/.vim/plugin```

##### Windows #####

1. create a directory at:

 ```C:\Users\YourUsername\vimfiles\plugin```

 or enter directory:

 ```C:\Program Files\vim\vim73\plugin```

 vim73 might be vim72 or whatever.. as long as it's where your vim is installed, it's valid.

2. copy plugin/randomColorPicker.vim to that directory.

### Usage ###
You will need to add the following line to your .vimrc file to pick the
next random colorscheme:

CSNext


* __ALL The Commands below are CaseSensitive__

* if you  __LOVE__  this colorscheme,

  Enter( In Normal Mode )

  `:Love`

  then I will never change your colorscheme again.

* if you __HATE__ this colorscheme and don't want to see her again,

  Enter( In Normal Mode )

  `:Hate`

  then I will never pick this colorscheme for you and then

  randomly pick a new colorscheme.

* if you somehow regret what you did and want to get the hated colorscheme back,

  Enter(In  Normal Mode)

  `:Back`

  then all you hated colorscheme will back to select pool, and you might see

  her again:)

* Enter(In Normal Mode)

  `:CS`

  to see current colorscheme

* Enter(In Normal Mode)

  `:CSnext`

  to switch to a new random theme without restarting vim.

#### Variables ####
* *g:colorscheme_user_path*

  Set to a comma-delimited string for Vim to look for colorschemes in additional areas, e.g.

  ```
  let g:colorscheme_user_path = '~/.vim/bundle/vim-colorschemes/colors'
  ```

  **NOTE:** This only works if Vim is aware of the other colorscheme paths, such as when you install colorscheme repositories using a plugin manager.

### Tips ###
This plugin is conservative in its _searching_ by default and will only look in your runtime path for colors. 
It _does_ include Base16 colours, but if you wish to override this behaviour, refer to the provided variables.

### Feedback is welcome
Adapted by blinklad for meme potential. Originally written by [Sunus Lee](mailto:sunus.the.dev@gmail.com)

