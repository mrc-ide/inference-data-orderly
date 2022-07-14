# inference-data-orderly

[![Build status](https://badge.buildkite.com/193017a1dbd38cc351c0bfc7da06662010827830916bfd851d.svg)](https://buildkite.com/mrc-ide/inference-data-orderly)

This is the docker container for [inference-data](https://github.com/mrc-ide/inference-data).

This repo is a fork of [`montagu-orderly`](https://github.com/vimc/montagu-orderly) with minor modifications

**Interaction with the server**.  These commands interact with the orderly server on the *same host* as you run it.  If you run these on your desktop they will not affect any other machine.

Make sure you have the most recent version of the container with

```
docker pull mrcide/inference-data-orderly:main
```

Update the `https://github.com/mrc-ide/inference-data` repo on the orderly volume

```
./pull_sources
```

Run orderly commands with

```
./orderly run <name>
./orderly list names
./orderly --help
```

etc.

Get a shell on the container with

```
./shell
```

## Building the image

The image is built on [Buildkite](https://buildkite.com/mrc-ide/hiv-orderly)
