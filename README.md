# Garage Env

>> Development environments with containers.

**ATENTION:** This is a work-in-progress.

### Why?

- Using your own box can get messy.
- Configuration is slow (download/build/install).
- Docker is cool.

## Instructions

```
$ curl -sSL https://raw.github.com/juniorz/garage-env/master/install | bash

# Installs Ruby 2.0 garage environment
$ garage get ruby20

$ garage run ruby -v

# Your cwd is automatically mounted as /garage inside the container
$ echo 'puts "It works!"' > foo.rb
$ garage run ruby foo.rb
> It works!

$ garage run irb
# now you have an IRB prompt

# Shows all executables available by all the installed garage environments
$ garage ls
> ruby
> irb

# TODO:
$ garage use ruby20
$ ruby -v # Ruby from garage env
```

### Requirements

- docker
- git

## Setting up your own garage

1. Set `$GARAGE_PROVIDES` to inform what your garage provides.
1. Assume your user's code will be placed into `/garage`.
2. Chroot your user to `/garage` and use `garage` user when possible.

**TODO**

## Acknowledgements

Garage Env is inspired by [baseline](https://github.com/bltavares/baseline) - but it's better!
