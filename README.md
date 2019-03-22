[Tiny Tiny RSS](https://git.tt-rss.org/git/tt-rss) is a self-hosted web-based RSS feed reader.

This docker config uses [this image](https://hub.docker.com/r/linuxserver/tt-rss/) from [LinuxServer.io]

# Setup

This relies on my [base docker services](https://github.com/StarlitGhost/selfhost-base).  
You'll want to symlink that project's .env file into this project's directory and set `POSTGRES_USER` and `POSTGRES_PW` in it.

Once that's done you can just spin it up. The remainder of the setup is done online at `rss.${DOMAIN_BASE}`
