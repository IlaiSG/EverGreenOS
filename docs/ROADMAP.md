# EverGreenOS Development Roadmap

## Milestone 0 — Establish the build

- [ ] Choose and document the initial Debian release and image configuration.
- [ ] Create a reproducible AMD64 build using GitHub Actions.
- [ ] Publish build artefacts for testing.

## Milestone 1 — First boot

- [ ] Produce a bootable x86-64 image.
- [ ] Boot it in QEMU.
- [ ] Verify basic startup, display, keyboard input, and shutdown.

## Milestone 2 — Desktop foundation

- [ ] Select and configure the initial desktop environment.
- [ ] Apply Evergreen branding, wallpaper, fonts, and icons.
- [ ] Document installation and testing.

## Milestone 3 — Evergreen experience

- [ ] Begin replacing default desktop components with Evergreen interfaces.
- [ ] Investigate integration with EverGreenLM.
- [ ] Establish a stable update and release process.

## Development principle

Prioritise a repeatable build and a reliably booting system before adding extensive customisation.
