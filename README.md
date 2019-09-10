# wazo-python-rfc3986-packaging

Debian packaging for [python-rfc3986]("https://github.com/python-hyper/rfc3986) used in Wazo.

## Upgrading

To upgrade python-hyper

* Update the version number in the `VERSION` file
* Update the changelog using `dch -i` to the matching version
* Refresh patches
* Push the changes

## Building Locally

To build on a test environment before submitting a change to production the following procedure can be used.

```sh
debian/rules get-orig-source
debuild -us -uc
```
The `.deb` will be located in the parent directory.
