[![SWUbanner](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg)](https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md)


### Additional terms of use for users from Russia and Belarus

By using the code provided in these repositories you agree with the following:
* Russia has [illegally annexed Crimea in 2014](https://en.wikipedia.org/wiki/Annexation_of_Crimea_by_the_Russian_Federation) and [brought the war in Donbas](https://en.wikipedia.org/wiki/War_in_Donbas) followed by [full-scale invasion of Ukraine in 2022](https://en.wikipedia.org/wiki/2022_Russian_invasion_of_Ukraine).
* Russia has brought sorrow and devastations to millions of Ukrainians, killed hundreds of innocent people, damaged thousands of buildings, and forced several million people to flee.
* [Putin khuylo!](https://en.wikipedia.org/wiki/Putin_khuylo!)

### Glory to Ukraine! 🇺🇦

# Unbound

[![Travis Build Status](https://travis-ci.org/NLnetLabs/unbound.svg?branch=master)](https://travis-ci.org/NLnetLabs/unbound)
[![Packaging status](https://repology.org/badge/tiny-repos/unbound.svg)](https://repology.org/project/unbound/versions)
[![Fuzzing Status](https://oss-fuzz-build-logs.storage.googleapis.com/badges/unbound.svg)](https://bugs.chromium.org/p/oss-fuzz/issues/list?sort=-opened&can=1&q=proj:unbound)

Unbound is a validating, recursive, caching DNS resolver. It is designed to be
fast and lean and incorporates modern features based on open standards. If you
have any feedback, we would love to hear from you. Don’t hesitate to
[create an issue on Github](https://github.com/NLnetLabs/unbound/issues/new)
or post a message on the [Unbound mailing list](https://lists.nlnetlabs.nl/mailman/listinfo/unbound-users).
You can lean more about Unbound by reading our
[documentation](https://nlnetlabs.nl/documentation/unbound/).

## Compiling

Make sure you have the C toolchain, OpenSSL and its include files, and libexpat
installed. Unbound can be compiled and installed using:

```
./configure && make && make install
```

You can use libevent if you want. libevent is useful when using many (10000)
outgoing ports. By default max 256 ports are opened at the same time and the
builtin alternative is equally capable and a little faster.

Use the `--with-libevent=dir` configure option to compile Unbound with libevent
support.

## Unbound configuration

All of Unbound's configuration options are described in the man pages, which
will be installed and are available on the Unbound
[documentation page](https://nlnetlabs.nl/documentation/unbound/).

An example configuration file is located in
[doc/example.conf](https://github.com/NLnetLabs/unbound/blob/master/doc/example.conf.in).
