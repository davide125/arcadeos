# ArcadeOS

ArcadeOS is an appliance-style OS for arcade cabinets based on
[ParticleOS](https://github.com/systemd/particleos).

The ArcadeOS image is built using [mkosi](https://github.com/systemd/mkosi). To
build the image, run `./mkosi -f` from the ArcadeOS repository.

It's recommended to set a root password (e.g. via `mkosi.rootpw` or
`RootPassword=` in `mkosi.local.conf`), as otherwise `systemd-firstboot` will
prompt for one on startup, but the prompt won't be visible due to the boot
splash unless that's dismissed.
