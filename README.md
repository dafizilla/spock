Spock for OSX 64bit
---------------

This fork contains the binary for OSX 64 bit and runs on Snow Leopard and Lion

It is a quick and dirty (really dirty) solution to run spock on Apple OSX, libraries are put on same spock's directory (a really ugly approach but it works so WHO CARES??)

The ruby script has been modified to use xmlstarlet because the libxml and libxslt versions installed from gem do not expand entities present on XSL sheet.

Adding disable-output-escaping to xsl:text/ tag produce a newline making the generated file unable to be parsed and I don't want to modify spock

Prerequisites
--

- starlet

I've used [homebrew] [1]: to install xmlstarlet

brew install xmlstarlet


[1]: https://github.com/mxcl/homebrew