# install_node

A bash script to install a version of node.js for a platform of your choosing,
without depending on nodejs.org being available.

## Usage

```
$ install_node <version> <platform> <dir>
```

This will find the corresponding node.js version for the requested `platform`
(one of `linux`, `darwin`, `win32`), and drop it into the specified `dir`.

## Allowed Versions

See [`cache/node-versions`](https://github.com/mapbox/install-node/blob/master/cache/node-versions).

## Caveats

- Installs x64 versions on darwin and linux, and 32-bit on win32
- win32 version is nothing but `node.exe`. Plan accordingly.