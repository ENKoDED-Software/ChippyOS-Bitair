# Open source licenses

ChippyOS's own code is free to use but not open source: see its [license terms](LICENSE). The firmware also includes software that
others made and shared under open source licenses. Thank you to everyone below. Each part is included unchanged, except BIP
173's reference code, which the firmware follows in its own code.

The web installer at chippyos.com lists its own parts on its [Open source licenses](https://chippyos.com/licenses.html) page.

## In the ChippyOS firmware

- **ESP-IDF 5.5.6,** by Espressif Systems. The system the firmware runs on: Wi-Fi, networking, the web server, updates and the
  rest. Apache License 2.0: [read the license](licenses/Apache-2.0.txt).
- **Espressif's Wi-Fi and radio libraries,** by Espressif Systems, as ESP-IDF ships them. Apache License 2.0:
  [read the license](licenses/Apache-2.0.txt).
- **Mbed TLS.** Secure connections to pools and for updates, and the update signature check. Offered under the Apache License 2.0
  or the GPL 2.0 or later; used here under the Apache License 2.0: [read the license](licenses/Apache-2.0.txt).
- **FreeRTOS,** by Amazon.com, Inc. or its affiliates. Runs the firmware's tasks. MIT license:
  [read the license](licenses/FreeRTOS-Kernel-MIT.txt).
- **FreeRTOS's Xtensa port and the Xtensa processor support,** by Cadence Design Systems, Inc. and Tensilica Inc. MIT license:
  [read the license](licenses/Xtensa-port-Cadence-MIT.txt).
- **lwIP 2.2.0,** by the Swedish Institute of Computer Science and others. The networking. BSD 3-Clause license:
  [read the license](licenses/lwIP-BSD-3-Clause.txt).
- **wpa_supplicant,** by Jouni Malinen and contributors. Wi-Fi security. BSD 3-Clause license:
  [read the license](licenses/wpa_supplicant-BSD-3-Clause.txt).
- **FreeBSD's net80211,** by Atsushi Onoe and Sam Leffler, Errno Consulting; two of its files also carry a notice by Jouni
  Malinen. Part of Espressif's Wi-Fi library. BSD 2-Clause license: [read the license](licenses/FreeBSD-net80211-BSD-2-Clause.txt).
- **TLSF,** by Matthew Conte. Memory management. BSD 3-Clause license: [read the license](licenses/TLSF-BSD-3-Clause.txt).
- **http_parser,** from NGINX by Igor Sysoev, and Joyent, Inc. and other Node contributors. Reads web requests. MIT license:
  [read the license](licenses/http_parser-MIT.txt).
- **Two small ESP-IDF files,** by Linaro Limited and Thomas Moestl, with changes by others. BSD 2-Clause license:
  [read the license](licenses/ESP-IDF-files-BSD-2-Clause.txt).
- **newlib,** the C library, as Espressif's tools ship it. Its own permissive licenses: [read the licenses](licenses/newlib.txt).
  That file also covers parts made for other kinds of computers, two of them under the LGPL; those parts are not in ChippyOS.
  Six of newlib's memory and string functions, written for Xtensa processors, are by Tensilica Inc. MIT license:
  [read the license](licenses/Xtensa-port-Cadence-MIT.txt). This product includes software developed by the University of
  California, Berkeley and its contributors.
- **GCC's runtime libraries and code from its C++ library headers,** as Espressif's tools ship them. GPL 3.0 with the GCC Runtime
  Library Exception, which allows their use in ChippyOS, since ChippyOS is built with GCC. Two of those headers, used by ESP-IDF's
  NVS storage and C++ support code, also carry notices by Hewlett-Packard Company (1994) and Silicon Graphics Computer Systems,
  Inc. (1996 and 1996-1998): [read the notices](licenses/libstdc++-HP-SGI.txt).
- **Mozilla's list of trusted certificate authorities.** Used to check the certificates of pools and of updates. Mozilla Public
  License 2.0 ([read the license](https://mozilla.org/MPL/2.0/)); it covers this list only. Its source is
  [cacrt_all.pem in ESP-IDF 5.5.6](https://github.com/espressif/esp-idf/blob/v5.5.6/components/mbedtls/esp_crt_bundle/cacrt_all.pem):
  Mozilla's certificate data as of 25 February 2025, in the form [curl extracts](https://curl.se/docs/caextract.html).
- **BIP 173,** by Pieter Wuille and Greg Maxwell. The checksum of bitcoin addresses that start bc1: the coinbase check follows its
  reference code to confirm your pool pays your address. 2-clause BSD license:
  [read the license](licenses/BIP-173-BSD-2-Clause.txt).
