# Playground

[![Swift 3.1](https://img.shields.io/badge/swift-3.1-orange.svg?style=flat)](#)
[![Marathon](https://img.shields.io/badge/marathon-compatible-brightgreen.svg?style=flat)](https://github.com/johnsundell/marathon)
[![SPM](https://img.shields.io/badge/spm-compatible-brightgreen.svg?style=flat)](https://github.com/apple/swift-package-manager)
[![@johnsundell](https://img.shields.io/badge/contact-@johnsundell-blue.svg?style=flat)](https://twitter.com/johnsundell)

Welcome to `playground`, a Swift script that enables you to super quickly generate Swift playgrounds from the command line - with or without dependencies - for any supported platform.

It essentially provies a command line interface to [Xgen](https://github.com/johnsundell/xgen).

**Features**

- [X] Generate playgrounds in seconds.
- [X] Automatically reuse any playground created today, for easy code note taking.
- [X] Add dependencies to a playground with a simple command - no more fiddling with workspaces.
- [X] Supports iOS, macOS & tvOS.

## Usage

**Simply run `playground` and a new playground will be created and opened**

```
$ playground
```

You can also supply various arguments to customize your playground:

**Add a playground at a specific path**

```
$ playground -t ~/MyPlayground
```

**Add some dependencies to your playground**

```
$ playground -d ~/unbox/unbox.xcodeproj,~/files/files.xcodeproj
```

**Quickly get started with view code prototyping**

```
$ playground -v
```

**Specify what platform you want the playground to run on**

```
$ playground -p tvOS
```

*For all available options, run `$ playground -h`*

## Installation

The easiest way to install `playground` is using [Marathon](https://github.com/johnsundell/marathon):

```
$ marathon install johnsundell/playground
```

You can also install it using the Swift Package Manager:

```
$ git clone git@github.com:JohnSundell/Playground.git
$ cd Playground
$ swift build -c release -Xswiftc -static-stdlib
$ cp -f .build/release/Playground /usr/local/bin/playground
```

## Help, feedback or suggestions?

- [Open an issue](https://github.com/JohnSundell/Playground/issues/new) if you need help, if you found a bug, or if you want to discuss a feature request.
- [Open a PR](https://github.com/JohnSundell/Playground/pull/new/master) if you want to make some change to `playground`.
- Contact [@johnsundell on Twitter](https://twitter.com/johnsundell) for discussions, news & announcements about `playground` & other projects.
