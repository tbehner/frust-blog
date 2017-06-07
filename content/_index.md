+++
date = "2017-04-19T14:34:33+02:00"
description = "a find replacement with SQL-like syntax"
title = "frust"

+++

frust is a find replacement with SQL-like syntax.

*Note:* frust has a *pre-alpha* status and has a lot of bugs, issues and missing features.
We are grateful for every opened issue, pull request or idea.
Additionally this project was written while learning a good part of the [Rust programming language](https://www.rust-lang.org/en-US/).
Hence the quality of code will hopefully improve while learning more about Rust.

## Installation
### Install from source
Clone the repository to a desired location and then compile the binary with
```
cargo build --release
```
and move the executable somewhere on $PATH, for example
```
cp ./target/release/frust $HOME/bin
```

### Download binary

* [linux-amd64](/frust-blog/binaries/frust-v0.0.2) (Commit [65ab866](https://github.com/tbehner/frust/commit/65ab866991c197b32446446f1985eafdd2407730)) ([signature](/frust-blog/signatures/frust-v0.0.2.sign))
* [linux-armv7](/frust-blog/binaries/frust-armv7-v0.0.2) (Commit [65ab866](https://github.com/tbehner/frust/commit/65ab866991c197b32446446f1985eafdd2407730)) ([signature](/frust-blog/signatures/frust-armv7-v0.0.2.sign))

Alternatively check the releases on the github project for binaries of newer or older releases.

To check that the signature is correct and the binary was not altered in any way, import my public key
```
gpg --keyserver pgp.mit.edu --recv 35233ACB
```
and execute
```
gpg --verify frust-v0.0.1.sign frust-v0.0.1
```
to verify the signature of the binary.
