<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the Egeria project. -->

# Sample certificates

The `gensamplecerts.sh` script is used for generating self-signed certificates for testing.
Once the certificates are created, the script copies them into the right locations to be picked up by applications

## Set up to run

The `gensamplecerts.sh` script uses `openssl`.  The default version for Linux is ok, but the version on the Mac is `libressl` by default and you need to use `brew install openssl@3` to install the genuine openssl library and then:

```bash
$ export PATH="/usr/local/opt/openssl@3/bin:$PATH"
$ ./gensamplecerts.sh
```

It is possible to reset all of the counts by setting CA_CLEAN environment variable.  However, this should not be the normal process. 

## Using the certificates

**Note:** Any generated certs are provided as an example only and to support demos and must not be used for production.  They assume the hostname is "localhost" and do not work in a distributed setup.

----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Egeria project.
