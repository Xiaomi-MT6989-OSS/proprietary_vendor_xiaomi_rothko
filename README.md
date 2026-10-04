# rothko stock vendor/ODM — local extraction baseline

Generated from HyperOS OS3.0.307.0.WNNCNXM using the matching device tree's
current extract-utils configuration. The selection reuses the original rothko
list, removes absent/duplicate objects, and adds reviewed current stock HALs
and dependencies. `PROVENANCE.json` records input and extracted hashes.

The stock vendor was built against Android 14 / API 34 while the handset's
framework runs Android 16. ELF presence alone does not establish compatibility
with this native LineageOS 23.2 vendor image. Keep ELF, VINTF and policy checks
enabled; do not revive unverified legacy interface replacements.

No raw LK/preloader/bootloader firmware is included. Do not add generic
boot-control/UFS BootLU switching or a full stock firmware flash script.
TEE/RPMB access, boot-control/misc initialization and remaining inherited
device configuration require review before any device boot or installation.

This private local baseline has not passed ROM build or first-boot validation.
