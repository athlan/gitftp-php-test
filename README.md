# `git ftp` example

See project page:

https://github.com/git-ftp/git-ftp

## Usage
  
While development, just use for deployment:
```
$ git ftp push
```

See also Scopes sections to mantain more than 1 server (staging, development, production).

https://github.com/git-ftp/git-ftp/blob/develop/man/git-ftp.1.md#scopes

## Setup environment (first time)

1. Clone git-ftp anywhere:
  ```
  git clone https://github.com/git-ftp/git-ftp
  ```
  
  Grant x permissions:
  ```
  cd git-ftp && chmod +x git-ftp
  ```

2. Create symlink to be visible in `$PATH`
  ```
  $ ln -s /bin/git-ftp /path/to/your/git-ftp/git-ftp
  ```
  or
  ```
  $ ln -s /usr/local/bin/git-ftp /path/to/your/git-ftp/git-ftp
  ```

## Setup in project

1. Initialize your gitftp settings
  ```
  $ git config git-ftp.user john
  $ git config git-ftp.url ftp.example.com
  $ git config git-ftp.password secr3t
  ```

2. Initialize git ftp on remote server
  ```
  $ git ftp init
  ```

