[Tiny Tiny RSS](https://git.tt-rss.org/git/tt-rss) is a self-hosted web-based RSS feed reader.

This docker config uses [this image](https://hub.docker.com/r/linuxserver/tt-rss/) from [LinuxServer.io](https://LinuxServer.io)

# Setup

This relies on my [base docker services](https://github.com/StarlitGhost/selfhost-base) and 
[postgres](https://github.com/StarlitGhost/selfhost-postgres).
You'll want to symlink selfhost-base's .env file into this project's directory.

With postgres running you'll want to run the following to create an empty database:

`docker exec -it postgres createdb -U docker ttrss`

Once that's done you can just spin it up with `docker-compose up -d`. The remainder of the setup is done online at `rss.${DOMAIN_BASE}`
