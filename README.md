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

- Download the latest release of `peco-docker` [here](https://github.com/YungSang/peco-docker/releases/latest).

```
$ cd /path/to/download
$ chmod +x peco-docker
$ mv peco-docker  /path/to/bin # in your $PATH
```

You can name it as you want.

```
$ alias deco="peco-docker"
```

### Usage

```
$ peco-docker help
Usage: peco-docker <command> [OPTIONS]

command:
  search         Search Docker images in the Docker registry
  pull           Search Docker images and download the selected images

  images [-a]    List the selected images in your Docker host (tcp://localhost:2375)
  tag            Tag the first selected image
  push           Push the selected images to the Docker registry
  rmi [-f]       Remove the selected images
  inspecti [-f]  Show low-level information on the selected images

  ps [-a]        List the selected containers in your Docker host (tcp://localhost:2375)
  start          Start the selected stopped containers
  restart        Restart the selected running containers
  stop           Stop the selected running containers
  kill           Kill the selected running containers
  rm [-f]        Remove the selected containers
  inspect [-f]   Show low-level information on the selected containers
  top            Lookup the processes of the selected running containers
  logs           Fetch the logs of the first selected container

  help           Show this message
```

```
$ peco-docker search
Usage: peco-docker search <term>
```

```
$ peco-docker pull
Usage: peco-docker pull <term to search> [tag]
```

```
$ peco-docker tag
Usage: peco-docker tag <name>[:tag]
```

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)  
To the extent possible under law, the person who associated CC0 with this work has waived all copyright and related or neighboring rights to this work.

- [peco](https://github.com/peco/peco): Copyright (c) 2014 lestrrat, under the [MIT License](https://github.com/peco/peco/blob/master/LICENSE)
- [Docker](http://www.docker.com) is under the [Apache 2.0 license](https://github.com/dotcloud/docker/blob/master/LICENSE).
- [pecrant](https://github.com/gongo/pecrant) is under the [MIT License](https://github.com/gongo/pecrant/blob/master/README.md).
