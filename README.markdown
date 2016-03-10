[![Build Status](https://travis-ci.org/jedisct1/libsodium.png?branch=master)](https://travis-ci.org/jedisct1/libsodium?branch=master)
[![Coverity Scan Build Status](https://scan.coverity.com/projects/2397/badge.svg)](https://scan.coverity.com/projects/2397)

![libsodium](https://raw.github.com/jedisct1/libsodium/master/logo.png)
============

Sodium is a new, easy-to-use software library for encryption,
decryption, signatures, password hashing and more.

It is a portable, cross-compilable, installable, packageable
fork of [NaCl](http://nacl.cr.yp.to/), with a compatible API, and an
extended API to improve usability even further.

Its goal is to provide all of the core operations needed to build
higher-level cryptographic tools.

Sodium supports a variety of compilers and operating systems,
including Windows (with MingW or Visual Studio, x86 and x64), iOS and Android.

## Documentation

The documentation is a work-in-progress, and is being written using
Gitbook:

[libsodium documentation](https://download.libsodium.org/doc/)

## Community

A mailing-list is available to discuss libsodium.

In order to join, just send a random mail to `sodium-subscribe` {at}
`pureftpd` {dot} `org`.

## License

[ISC license](https://en.wikipedia.org/wiki/ISC_license).

## Wire Fork

The Wire fork differs from upstream only in that it exposes several
additional functions in the Emscripten build.

The additional functions are as follows:

 - `crypto_hash_sha256`
 - `crypto_hash_sha256_bytes`
 - `crypto_auth_hmacsha256`
 - `crypto_auth_hmacsha256_verify`
 - `crypto_auth_hmacsha256_bytes`
 - `crypto_auth_hmacsha256_keybytes`
 - `crypto_auth_hmacsha512`
 - `crypto_auth_hmacsha512_verify`
 - `crypto_auth_hmacsha512_bytes`
 - `crypto_auth_hmacsha512_keybytes`
 - `crypto_stream_chacha20_xor`
 - `crypto_stream_chacha20_xor_ic`
 - `crypto_stream_chacha20_noncebytes`
 - `crypto_stream_chacha20_keybytes`
