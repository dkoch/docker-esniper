## Summary
Fork of [Michael Rüttger's dockerized esniper version](https://github.com/mruettgers/docker-esniper),
changed to work with mounted config files instead of command line arguments.

## Usage
    docker run -d --rm -v /local/config/directory:/var/lib/esniper/config dieterkoch/docker-esniper

## Config files
The image expects two files in the mounted directory: a configuration file named
`esniper.conf` and an auction file named `auctions`. Information
on the layouts of both files can be found in [the manual](http://esniper.sourceforge.net/esniper_man.html).
