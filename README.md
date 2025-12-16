<p align="center">
  <h1 align="center">BoringOS</h1>
  <p align="center"><strong>Your computer. Minus the nonsense.</strong></p>
  <p align="center">
    <a href="https://github.com/getboring/boringos/actions/workflows/build.yml"><img src="https://github.com/getboring/boringos/actions/workflows/build.yml/badge.svg" alt="Build Status"></a>
    <a href="https://boringos-site.vercel.app"><img src="https://img.shields.io/badge/Website-boringos-orange" alt="Website"></a>
    <a href="https://github.com/getboring/boringos/blob/main/LICENSE"><img src="https://img.shields.io/github/license/getboring/boringos" alt="License"></a>
  </p>
</p>

---

Same computer. Same files. Same apps.
**No ads. No tracking. No forced updates.**

BoringOS is an auto-updating Fedora Atomic image that just works.

---

## ✓ What You Get

| | |
|---|---|
| **Firefox** | Browse the internet |
| **Thunderbird** | Check your email |
| **LibreOffice** | Documents, spreadsheets, presentations |
| **Photos & Videos** | View and play your media |
| **Music** | Your library, your way |
| **Games** | Chess, Solitaire, Sudoku — no ads |
| **Kids Apps** | GCompris educational activities |

Everything you need. Nothing you don't.

---

## ✗ What You'll Never See

- ~~"Your PC doesn't meet requirements"~~ — Runs on computers Windows rejected
- ~~Ads in your Start menu~~ — No ads. Anywhere. Ever.
- ~~"Restart now to update"~~ — Updates when you want
- ~~"Sign in with Microsoft"~~ — No account required
- ~~"Give Edge a chance"~~ — No nagging
- ~~Virus warnings~~ — Doesn't get viruses

---

## Installation

> [!NOTE]
> BoringOS replaces your current operating system. Back up your files first.

### From Fedora Atomic

```bash
# 1. Rebase to unsigned image
rpm-ostree rebase ostree-unverified-registry:ghcr.io/getboring/boringos:latest

# 2. Reboot
systemctl reboot

# 3. Rebase to signed image
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/getboring/boringos:latest

# 4. Reboot again
systemctl reboot
```

Done.

---

## Verification

Images are signed with [Sigstore](https://www.sigstore.dev/) cosign:

```bash
cosign verify --key cosign.pub ghcr.io/getboring/boringos
```

---

## Built With

<a href="https://fedoraproject.org/silverblue/"><img src="https://img.shields.io/badge/Fedora-Silverblue-blue" alt="Fedora Silverblue"></a>
<a href="https://universal-blue.org"><img src="https://img.shields.io/badge/Universal-Blue-blue" alt="Universal Blue"></a>
<a href="https://blue-build.org"><img src="https://img.shields.io/badge/Blue-Build-blue" alt="BlueBuild"></a>

---

<p align="center"><strong>Free forever.</strong></p>
