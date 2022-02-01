# Homebrew-git-curl-openssl

A formula for `git` with `curl` and `openssl@1.1`.

The default `git` formula links libcurl from macOS, and that library currently does not support TLSv1.3.

This formula allows git to connect to https with TLSv1.3.

## Installation

Uninstall `git` if you have it installed already to allow linking this formula:

```shell
brew uninstall git
```

Install this formula and build it from source with `curl-openssl`:

```shell
brew tap digitalfish/git-curl-openssl
brew install -s git-curl-openssl
```
