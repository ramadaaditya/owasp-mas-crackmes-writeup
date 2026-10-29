# OWASP MAS Crackmes — Write-ups & Solutions

> Personal learning notes and reproducible solutions for the [OWASP MAS Crackmes](https://mas.owasp.org/crackmes/) mobile reverse-engineering challenges.

[![Platform](https://img.shields.io/badge/platform-Android%20%7C%20iOS-informational)](https://mas.owasp.org/crackmes/)
[![Focus](https://img.shields.io/badge/focus-Mobile%20Security-blue)](https://mas.owasp.org/)
[![Status](https://img.shields.io/badge/status-learning%20project-lightgrey)]()

## About

This repository documents my own methodology, observations, and solutions for OWASP MAS Crackmes / UnCrackable Apps. The challenges are educational exercises referenced by the OWASP Mobile Application Security Testing Guide (MASTG).

**Spoiler warning:** write-ups may reveal challenge logic, secrets, and bypass approaches. Try each challenge yourself before reading the solution.

## Challenge index

| Challenge | Platform | Focus (initial hypothesis) | Status | Write-up |
|---|---|---|---|---|
| Android UnCrackable L1 | Android | Static/dynamic analysis, basic anti-tampering | Not started | [Open](writeups/android/uncrackable-l1/README.md) |
| Android UnCrackable L2 | Android | Java + native code analysis | Not started | [Open](writeups/android/uncrackable-l2/README.md) |
| Android UnCrackable L3 | Android | Native code, obfuscation, anti-tampering | Not started | [Open](writeups/android/uncrackable-l3/README.md) |
| Android UnCrackable L4 / r2pay | Android | PIN/salt validation, white-box crypto (version-dependent) | Not started | [Open](writeups/android/uncrackable-l4/README.md) |
| Android License Validator | Android/Linux ELF | Serial validation, native analysis | Not started | [Open](writeups/android/license-validator/README.md) |
| Android UnCrackable DRM | Android/Linux ELF | Native binary analysis | Not started | [Open](writeups/android/uncrackable-drm/README.md) |
| iOS UnCrackable L1 | iOS | Static/dynamic analysis | Not started | [Open](writeups/ios/uncrackable-l1/README.md) |
| iOS UnCrackable L2 | iOS | Static/dynamic analysis, native code | Not started | [Open](writeups/ios/uncrackable-l2/README.md) |

> Challenge names and available downloads may change. Check the official [MAS Crackmes index](https://mas.owasp.org/crackmes/) before starting.

## Repository structure

```text
.
├── README.md
├── CONTRIBUTING.md
├── DISCLAIMER.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── methodology.md
│   └── tools.md
├── templates/
│   └── WRITEUP_TEMPLATE.md
├── writeups/
│   ├── android/
│   │   ├── uncrackable-l1/README.md
│   │   ├── uncrackable-l2/README.md
│   │   ├── uncrackable-l3/README.md
│   │   ├── uncrackable-l4/README.md
│   │   ├── license-validator/README.md
│   │   └── uncrackable-drm/README.md
│   └── ios/
│       ├── uncrackable-l1/README.md
│       └── uncrackable-l2/README.md
└── assets/
    └── screenshots/
```

## Suggested workflow

1. Read the challenge description and attempt it without spoilers.
2. Record device/OS, app version, hash, and tool versions.
3. Start with static analysis; move to dynamic analysis when it adds evidence.
4. Document observations before conclusions.
5. Include commands/scripts only when you can explain what they do.
6. Re-test the solution from a clean install and record expected output.
7. Link official references and relevant MASTG test cases where applicable.

## Tooling

Tool choices vary by challenge. Common options include:

- **Static:** JADX, apktool, MobSF, Ghidra, radare2/rizin, `strings`, `readelf`, `file`
- **Dynamic:** adb, Frida, jdb, LLDB, objection (where appropriate)
- **iOS:** class-dump alternatives, Ghidra/Hopper, LLDB, Frida, Xcode tooling
- **Evidence:** terminal output, screenshots, hashes, minimal reproducible scripts

See [docs/tools.md](docs/tools.md) and [docs/methodology.md](docs/methodology.md).

## References

- [OWASP MAS Crackmes](https://mas.owasp.org/crackmes/)
- [OWASP MAS Crackmes source repository](https://github.com/OWASP/mas-crackmes)
- [OWASP MASTG](https://mas.owasp.org/MASTG/)
- [OWASP MASVS](https://mas.owasp.org/MASVS/)

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Corrections, additional approaches, and reproducibility improvements are welcome.

## License and third-party content

This repository is a collection of original notes and references. Do not commit challenge APKs/IPAs, proprietary binaries, or third-party write-ups unless the applicable license explicitly permits redistribution. Link to official downloads instead. See [DISCLAIMER.md](DISCLAIMER.md) and the original project's licensing terms.
