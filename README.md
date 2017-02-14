# megaput docker image #

## Description ##

Docker image to upload local files to a mega.nz cloud drive.

Uses [ubuntu](https://hub.docker.com/_/ubuntu/) base image with [megatools](https://github.com/megous/megatools) for uploads.

## Usage ##

```bash
$ docker run -it --rm -v "$(pwd)":/workdir -w /workdir klutchell/megaput \
--username "testuser@email.com" \
--password "topsecret" \
--path "/Root/backups" \
"file/to/upload"
```

## Parameters ##

See the [megaput man page](https://megatools.megous.com/man/megaput.html).

Note that only files within current directory and subdirectories will be available.

## Author ##

* Kyle Harding <kylemharding@gmail.com>

## Credit ##

I give credit where it's due and would like to give a shoutout to the creators of the utilites/images used in this project:
* [megous](https://github.com/megous/)
