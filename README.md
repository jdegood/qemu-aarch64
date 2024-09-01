# qemu-aarch64

Scripts to create, release, and use a Debian aarch64 (arm64) VM on QEMU.

Useful for education, e.g., learning aarch64 assembly language
on an x86-64 host.

Host port 5555 is forwarded to aarch64 guest port 22 (ssh), so
from a host command prompt:

* copy file from aarch64 guest to host
    * scp -P 5555 username@localhost:guest-file-path host-file-path

* copy file from host to aarch64 guest
    * scp -P 5555 host-file-path username@localhost:guest-file-path
