# go-mod-vendor

Vendor dependencies with Go 1.11's modules.

**Disclaimer:** I only intend to use and maintain this until modules make it
out of experimental and the tooling catches up. There are a lot of people
already working very hard on this stuff, and it shouldn't be too long before
this script is no longer needed.

## Y?

I've been playing around with modules since they were announced. The experience
has been great, but all my tooling has been broken.

While we were at GopherCon, my friend
[@ryanfaerman](https://github.com/ryanfaerman) had the bright idea to just use
the `mod` subcommand to vendor his dependencies.

Fast forward a couple of days and I decided to try and see if this would work
for me. Sure enough, I was able to vendor everything and my tooling works.

This flow gets annoying to type, so I put it into a shell script.

## Quick Start

```
$ curl -o $SOMEWHEREINYOURPATH/go-mod-vendor https://raw.githubusercontent.com/juicemia/go-mod-vendor/master/go-mod-vendor
$ chmod 755 $SOMEWHEREINYOURPATH/go-mod-vendor
```
