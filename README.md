# php-vimparse

# Install

> composer global require ha1t/php-vimparse

```vim
" @see http://subtech.g.hatena.ne.jp/secondlife/20080729/1217315593
if executable('vimparse.php')
  setlocal makeprg=vimparse.php\ %\ $*
  setlocal errorformat=%f:%l:%m
  setlocal shellpipe=2>&1\ >
  autocmd BufWritePost <buffer> silent make
endif
```

