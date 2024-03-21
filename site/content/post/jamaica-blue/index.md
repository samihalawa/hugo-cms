---
title: Scrappy - Talk to your Codebase. Use ChatGPT with Github
date: 2017-01-04T15:04:10.000Z
description: We’re proud to announce that we’ll be offering a small batch of
  Jamaica Blue Mountain coffee beans in our store next week.
---


![Scrappy Scrappy Doo.](screenshot-2024-03-21-at-16.42.28.png)

Scrappy is a simple CLI tool that helps you collect and format code from a directory structure, making it easy to ask questions on platforms like ChatGPT by providing complete code context. With Scrappy, you can quickly generate a single Markdown file containing all the code from a module or project, so you don't have to manually copy and paste each file.

[![Test](https://github.com/WezSieTato/scrappy/actions/workflows/test.yml/badge.svg)](https://github.com/WezSieTato/scrappy/actions/workflows/test.yml)

## Table of Contents

* [Installation](#installation)
* [Usage](#usage)
* [Development](#development)
* [Testing](#testing)
* [Acknowledgements](#acknowledgements)
* [License](#license)

## Installation

### From source code

To install Scrappy, make sure you have [Rust](https://www.rust-lang.org/tools/install) installed, and then run the following command:

```sh
cargo install --path .
```

### Homebrew

```sh
brew tap WezSieTato/scrappy
brew install scrappy
```

## Usage

To use Scrappy, navigate to the directory containing the code you want to compile and run the following command:

```sh
scrappy <source_directory> <output_file>
```

For example:

```sh
scrappy ./src output.md
```

This will generate an output.md file with the code from all the files in the src directory.

## Development

To contribute to the development of Scrappy, clone the repository and navigate to the project directory:

```sh
git clone https://github.com/WezSieTato/scrappy.git
cd scrappy
```

Then, build the project using Cargo:

```sh
cargo build
```

## Testing

To run the test suite for Scrappy, use the following command:

```sh
cargo test
```