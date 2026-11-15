# Byard packages

The package registry for [Byard](https://github.com/Briany4717/byard), served at
**https://packages.byard.dev**.

```sh
byard add material --registry https://packages.byard.dev
```

It's a folder of files: `index.toml` lists every published version with its checksum
and dependencies, and each version is an archive under its package's name
(`material/0.1.0.tar.gz`). `byard publish` writes both, and a push to `main` serves
them. Nothing here is built.

A published version is never replaced. A fix is a new version.
