# Building EverGreenOS

## Current build method

The initial AMD64 live image is assembled with Debian Live Build in a GitHub Actions runner. The runner is a temporary build machine; the resulting ISO is uploaded as a workflow artifact.

## Triggering a build

1. Open the repository's **Actions** tab.
2. Select **Build EverGreenOS ISO**.
3. Choose **Run workflow** on the `main` branch, or push a change under `distribution/`.

## Expected artifact

A successful run uploads an artifact named `evergreenos-amd64-iso`. Download and extract it to obtain the ISO image.

## Testing

Boot the ISO in QEMU. Check that it starts, reaches the graphical desktop, accepts keyboard input and shuts down cleanly. Emulator success is not proof of compatibility with every physical PC.

## Build troubleshooting

Read the first meaningful error in the **Build ISO** job. Later chroot errors can be secondary effects of an earlier bootstrap or package-download failure. Fix the earliest root cause rather than treating the final error as the cause.
