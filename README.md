# docker-react-cli

Because we are using `Docker` this image will provide `react` cli
commands like `create-react-app`, `create-react-native-app`,
`react-native-cli`, etc without having to install `node`, or these
packages in your development machine.

## Usage

1. You can clone this repo and build your own image

```sh
$ git clone https://github.com/przbadu/docker-react-cli.git
$ cd docker-react-cli
$ docker build . -t docker-react-cli
```

2. Use your image to generate scaffold

For Linux/Mac

```sh
$ docker run -v ${PWD}:/app docker-react-cli create-react-app myApp
```

For Windows

```sh
$ docker run -v %cd%:/app docker-react-cli create-react-app myApp
```

> NOTE: you can also use my docker image `przbadu/docker-react-cli`.
