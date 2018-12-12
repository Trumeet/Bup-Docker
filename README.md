[![](https://img.shields.io/docker/build/thnuiwelr/bup-docker.svg)](https://hub.docker.com/r/thnuiwelr/bup-docker/)
[![](https://img.shields.io/docker/pulls/thnuiwelr/bup-docker.svg)](https://hub.docker.com/r/thnuiwelr/bup-docker/)
[![](https://img.shields.io/microbadger/image-size/thnuiwelr/bup-docker.svg)](https://hub.docker.com/r/thnuiwelr/bup-docker/)

# Bup-Docker
This is an unoffical docker implementation for [Bup](https://github.com/bup/bup).

# Usage
It wraps a bup program, you can just replace any `bup` command to `docker run --rm thnuiwelr/bup-docker`.

Demo: to init a backup folder:

```shell
$ docker run \
    -v /path/to/backup:/root/Backup:rw \
    thnuiwelr/bup-docker \
    -d /root/Backup \
    init
```

# License
WTFPL - Don't worry about it.
