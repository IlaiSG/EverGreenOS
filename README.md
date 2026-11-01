# EverGreenOS

**EverGreenOS** is an independently designed desktop operating system built on the Linux kernel, with Debian providing the initial distribution and package-management foundation.

Our ambition is a coherent, integrated computing experience: first-party Evergreen desktop software, system settings, services and applications, built on dependable low-level infrastructure.

## Project principles

- **Evergreen identity:** Debian is the foundation, not the product identity.
- **Practical engineering:** use proven components where they serve us well; build first-party components where they create a real advantage.
- **Replaceable layers:** keep the Evergreen experience distinct from the underlying distribution.
- **Test before claiming:** boot images in QEMU and document what has actually been tested.

## Initial technical direction

- Linux kernel
- Debian 13 (Trixie) foundation
- AMD64 live image first
- Debian Live Build and GitHub Actions for reproducible image creation
- XFCE as a temporary graphical baseline while the Evergreen desktop is developed

## First milestone

Produce a reproducible, bootable AMD64 ISO, identify itself as EverGreenOS, and test it in QEMU. The current image is an experimental development build, not a production release.

## Repository map

- `distribution/` — live-image configuration and package selection
- `desktop/` — plans and, later, first-party desktop implementation
- `docs/` — architecture, roadmap and build instructions
- `.github/workflows/` — automated builds

## Build

See [docs/building.md](docs/building.md) for instructions.

## Status

Early development. A successful build and emulator test are still required before the first milestone can be considered complete.
