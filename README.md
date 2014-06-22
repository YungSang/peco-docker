# peco-docker

Docker helper powered by peco, inspired by [pecrant](https://github.com/gongo/pecrant)

## Requirements

- [peco](https://github.com/peco/peco)
- [Docker](http://www.docker.com)

```
$ docker search <image-name> | peco
$ docker images -a | peco
$ docker ps -a | peco
```

## Getting started

### Installation

```
$ cd /path/to/bin # in your $PATH
$ curl -OL https://raw.githubusercontent.com/YungSang/peco-docker/master/peco-docker
$ chmod +x ./peco-docker
```

You can name it as you want.

```
$ alias deco="peco-docker"
```

### Usage

```
$ peco-docker help
Usage: peco-docker <command>

  search  Search Docker images
  pull    Search Docker images and download the selected images
  help    Show this message
```

```
$ peco-docker search
Usage: peco-docker search <image-name>
```

```
$ peco-docker pull
Usage: peco-docker pull <image-name>
```

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)  
To the extent possible under law, the person who associated CC0 with this work has waived all copyright and related or neighboring rights to this work.

- [peco](https://github.com/peco/peco): Copyright (c) 2014 lestrrat, under the [MIT License](https://github.com/peco/peco/blob/master/LICENSE)
- [Docker](http://www.docker.com) is under the [Apache 2.0 license](https://github.com/dotcloud/docker/blob/master/LICENSE).
- [pecrant](https://github.com/gongo/pecrant) is under the [MIT License](https://github.com/gongo/pecrant/blob/master/README.md).
