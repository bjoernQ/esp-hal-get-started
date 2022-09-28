# Introduction

The goal of this book is to provide a getting-started guide on using the Rust programming language with Espressif SoCs and modules using [esp-hal](https://github.com/esp-rs/esp-hal).

## The Two Approaches

First thing to decide when approaching Rust on Espressif SoCs is which approach you are going to use. We provide two very
different ways to run your Rust code. (Actually there are three ways)

- Running in a hosted environment: use Rust including [libstd](https://doc.rust-lang.org/std/) on top of [ESP-IDF](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/index.html/) - this matches the approach outlined [here](https://docs.rust-embedded.org/book/intro/no-std.html#hosted-environments)
- Running in a bare metal environment: use Rust without [libstd](https://doc.rust-lang.org/std/) and memory allocations are optionally supported - this matches the approach outlined [here](https://docs.rust-embedded.org/book/intro/no-std.html#bare-metal-environments)

This book will only cover the second approach. To learn more about the first approach please follow the instructions found in [The Rust on ESP book](https://esp-rs.github.io/book/overview/using-the-standard-library.html)

## What is not covered?

In this book we will cover the basics using the most standard tools.

For many things there are alternative ways and tools but especially in the beginning that might be confusing.

Examples shown here usually apply to ESP32-C3 using the [ESP32-C3-DevKit-RUST-1](https://github.com/esp-rs/esp-rust-board) board.

You can use any other ESP32, ESP32-C3, ESP32-S2 or ESP32-S3 development board but smaller code changes and configuration changes might be needed.

Also this book will only cover working locally. But there is support to use [dev-containers](https://esp-rs.github.io/book/dependencies/installing-rust.html#using-containers) and even developing in a hosted cloud environment like GitHub Codespaces and GitPod. 

Additionally you can even try running code in a web browser without any actualy hardware using [Wokwi](https://wokwi.com/rust)

## Important Terminology

This book assumes you are familiar with some special terms. If you don't already know what a PAC or HAL is there is a good introduction in the [Discovery Book](https://docs.rust-embedded.org/discovery/microbit/04-meet-your-hardware/terminology.html)
