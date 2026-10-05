<div align="center">
<h1>trivalent-ci</h1>
</div>

This is a repository for updating the `trivalent-bin` AUR package. It does SLSA and GPG attestation checks before pushing an updated version of the PKGBUILD. Doing these checks locally is redundant due to the sha256sums and the fact that a compromised PKGBUILD means you're screwed regardless.

## Versioning scheme

Since there can be updates that only change the patch revision (after the -), and the AUR won't let me use the `pkgrel` to hold the patch number, I simply bump the `pkgrel` for those smaller patch releases. It's not the most visible solution to users but it works.

Normal Chromium updates change the `pkgver` and reset the `pkgrel` to 1, as per AUR policy.

## Issues

Please make an issue here or comment on the AUR page if something isn't working, and only flag the package out of date if it hasnt been updated in a few hours after the upstream release.

