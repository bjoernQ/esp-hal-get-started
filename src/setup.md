# Setting up a development environment

## Installing Rust

Depending on which target you want to use installing Rust can be more or less involved.

Please follow the instructions outlined in [The Rust on ESP Book](https://esp-rs.github.io/book/dependencies/installing-rust.html)

## Installing Tools

There are only a few tools needed to get started.

* cargo-generate (`cargo install cargo-generate`)
    - used to create a new project from a template, this is not strictly needed but creating a new project from scratch is quite some work
* espflash (`cargo install espflash`)
    - used to flash your code via USB-serial

There are other tools which might be useful (e.g. `espmonitor`) but these two are the bare-minimum to follow the instructions in this book.

It's assumed you use [Visual Studio Code](https://code.visualstudio.com/) with the [Rust Analyzer Extension](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer) but that is not strictly needed and in theory you could use any text editor.
