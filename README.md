# PoC of CVE-2023-4911 "Looney Tunables"

This is a PoC of CVE-2023-4911 (a.k.a. "Looney Tunables") exploiting a bug in glibc dynamic loader's `GLIBC_TUNABLES` environment variable parsing function `parse_tunables()`.

Code has been tested on Ubuntu 22.04.3 with glibc version `2.35-0ubuntu3.3`. No attempts have been made to generalize the PoC (read: "Works On My Machine"), so your mileage may vary.

As always, big kudos to the [Qualys Threat Research Unit](https://www.qualys.com/tru/) for the discovery of the vulnerability and for the [very detailed writeup](https://seclists.org/oss-sec/2023/q4/18).

-----

Written by [Xion](https://twitter.com/0x10n) of [KAIST Hacking Lab](https://kaist-hacking.github.io/)
