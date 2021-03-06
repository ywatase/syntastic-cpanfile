# syntastic-cpanfile

cpanfile syntax checker for [syntastic](https://github.com/scrooloose/syntastic)


# How to install

## Using [NeoBundle][nb]

1. Add `NeoBundle 'moznion/syntastic-cpanfile'` to `~/.vimrc`
2. Re-open vim or execute `:source ~/.vimrc`

## Using [vim-plug][vp]

1. Add `Plug 'moznion/syntastic-cpanfile'` to `~/.vimrc`
2. `:PlugInstall` or `$ vim +PlugInstall +qall`

## By Hand

Add symbolic link to syntax\_checkers/cpanfile  
e.g.)

    (In syntastic-cpanfile directory;)
    ln -s `pwd`/syntax_checkers/cpanfile ~/.vim/bundle/syntastic/syntax_checkers/cpanfile

And also you can use a way to copy the directory. (Maybe this way is not good...)  
e.g.)

    (In syntastic-cpanfile directory;)
    cp -R syntax_checkers/cpanfile/ ~/.vim/bundle/syntastic/syntax_checkers/


# Configuration and Environment

Please configure into .vimrc like so;

    ...
    au BufNewFile,BufRead cpanfile set filetype=cpanfile
    au BufNewFile,BufRead cpanfile set syntax=perl.cpanfile
    ...


# Dependencies

- [Module::CPANfile](https://metacpan.org/release/Module-CPANfile)
- [syntastic](https://github.com/scrooloose/syntastic)


#License

MIT License

    Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
