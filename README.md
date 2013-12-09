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

$ garage get ruby20
$ garage ruby20 foo.rb

$ garage use ruby20
$ ruby -v # Ruby from garage env

$ garage get irb20
$ garage irb
$ (irb prompt)
```

### Requirements

- docker
- git

## Setting up your own garage

1. Assume your user's code will be placed into `/garage`.
2. Chroot your user to `/garage` and use `garage` user when possible.

**TODO**

## Acknowledgements

Garage Env is inspired by [baseline](https://github.com/bltavares/baseline) - but it's better!
