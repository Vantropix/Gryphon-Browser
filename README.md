Am a simple dev looking at browser code.
the name Gryphon Browser is not locked to me as i would be very surprised with myself if i manage to make a complete browser.

This is my own attempt at adding features on top of a browser that browser extensions can't.
Reason for chosing lady bird to do this instead of a chrome of firefox based solusion is simply cause i believe in what lady bird is doing and am hoping it will become mine and many others main or at least second or tertiary browser.
Feel free to look at anything i do here, use anything including names or anything i have made personally but please still comply with the original ladybird terms for things that belong to them.

Until i decide this project is worth something everything written here is CC0 Public Domain.
If you used anything before a change in licence it is also concidered CC0 Public Domain, no worries :3

original description below

# Ladybird

[Ladybird](https://ladybird.org) is a truly independent web browser, using a novel engine based on web standards.

> [!IMPORTANT]
> Ladybird is in a pre-alpha state, and only suitable for use by developers
>

## Features

We aim to build a complete, usable browser for the modern web.

Ladybird uses a multi-process architecture with a main UI process, several WebContent renderer processes,
an ImageDecoder process, and a RequestServer process.

Image decoding and network connections are done out of process to be more robust against malicious content.
Each tab has its own renderer process, which is sandboxed from the rest of the system.

At the moment, many core library support components are inherited from SerenityOS:

- LibWeb: Web rendering engine
- LibJS: JavaScript engine
- LibWasm: WebAssembly implementation
- LibCrypto/LibTLS: Cryptography primitives and Transport Layer Security
- LibHTTP: HTTP/1.1 client
- LibGfx: 2D Graphics Library, Image Decoding and Rendering
- LibUnicode: Unicode and locale support
- LibMedia: Audio and video playback
- LibCore: Event loop, OS abstraction layer
- LibIPC: Inter-process communication

## How do I build and run this?

See [build instructions](Documentation/BuildInstructionsLadybird.md) for information on how to build Ladybird.

Ladybird runs on Linux, macOS, Windows (with WSL2), and many other \*Nixes.

## How do I read the documentation?

Code-related documentation can be found in the [documentation](Documentation/) folder.

## Get in touch and participate!

Join [our Discord server](https://discord.gg/nvfjVJ4Svh) to participate in development discussion.

Please read [Getting started contributing](Documentation/GettingStartedContributing.md) if you plan to contribute to Ladybird for the first time.

Before opening an issue, please see the [issue policy](CONTRIBUTING.md#issue-policy) and the [detailed issue-reporting guidelines](ISSUES.md).

The full contribution guidelines can be found in [`CONTRIBUTING.md`](CONTRIBUTING.md).

## License

Ladybird is licensed under a 2-clause BSD license.
