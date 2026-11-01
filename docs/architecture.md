# EverGreenOS Architecture

## Product direction

EverGreenOS is an independently designed desktop operating system built on the Linux kernel. The initial release uses Debian as its distribution and package-management foundation. Debian is infrastructure, not the product identity.

The guiding idea is a coherent, integrated system: the desktop, system settings, services, applications and visual language should feel as though they belong to one operating system.

## Initial layers

1. **Evergreen experience** — branding, desktop defaults, applications and documentation.
2. **Evergreen desktop** — a future first-party shell and system UI, developed as a distinct project.
3. **System integration** — defaults, services, configuration and installer experience.
4. **Linux platform** — Linux kernel, drivers, systemd and established system utilities.
5. **Debian foundation** — package repositories, package management and initial live-image tooling.

## Engineering rules

- Prefer established, maintained components for low-level infrastructure.
- Build first-party components where they create a meaningful user-facing or engineering advantage.
- Keep each layer replaceable; avoid unnecessary dependence on Debian-specific internals in Evergreen applications.
- Test every image in an emulator before considering physical hardware.
- Do not claim hardware compatibility until it has been tested on that hardware.

## First release scope

The first milestone is deliberately modest: a reproducible AMD64 live ISO that boots, provides a graphical desktop, identifies itself as EverGreenOS and can be tested in QEMU.
