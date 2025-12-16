# BoringOS

[![Build Status](https://github.com/getboring/boringos/actions/workflows/build.yml/badge.svg)](https://github.com/getboring/boringos/actions/workflows/build.yml)

**Your computer. Minus the nonsense.**

BoringOS is an auto-updating Fedora Atomic image. Same computer. Same files. Same apps. No ads. No tracking. No forced updates.

**Website:** [boringos-site.vercel.app](https://boringos-site.vercel.app)

---

## Installation

> [!NOTE]
> BoringOS replaces your current operating system. Back up your files first.

### From an existing Fedora Atomic installation

1. Rebase to the unsigned image:
   ```
   rpm-ostree rebase ostree-unverified-registry:ghcr.io/getboring/boringos:latest
   ```

2. Reboot:
   ```
   systemctl reboot
   ```

3. Rebase to the signed image:
   ```
   rpm-ostree rebase ostree-image-signed:docker://ghcr.io/getboring/boringos:latest
   ```

4. Reboot again:
   ```
   systemctl reboot
   ```

Done. Your computer now runs BoringOS.

---

## What's Included

- Firefox (web browser)
- Thunderbird (email)
- LibreOffice (documents, spreadsheets, presentations)
- Photos, Videos, Music players
- Games (Chess, Solitaire, Sudoku)
- Educational apps for kids (GCompris)

Everything you need. Nothing you don't.

---

## Verification

Images are signed with [Sigstore](https://www.sigstore.dev/) cosign. Verify with:

```bash
cosign verify --key cosign.pub ghcr.io/getboring/boringos
```

---

## Built With

- [Fedora Silverblue](https://fedoraproject.org/silverblue/)
- [Universal Blue](https://universal-blue.org)
- [BlueBuild](https://blue-build.org)

---

**Free forever.**
