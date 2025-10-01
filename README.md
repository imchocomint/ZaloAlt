# In progress of merging between Pake versions. Development will be slow.


<h1 align="center">ZaloAlt</h1>
<p align="center"><strong>Alternative Zalo client built using <a href="https://www.rust-lang.org/">Rust</a>, <a href="https://tauri.app/">Tauri</a> and <a href="https://github.com/tw93/Pake">Pake</a>.</strong></p>
<div align="center">
    <a href="https://github.com/imchocomint/ZaloAlt/releases" target="_blank">
    <img alt="GitHub downloads" src="https://img.shields.io/github/downloads/imchocomint/ZaloAlt/total.svg?style=flat-square"></a>
</div>

<div align="left"></div>

# Features

- Lighter than the official Zalo app (in term of program size)
- Faster (probably)
- Never take your storage for granted
- Support Linux**

** see Bugs

# What it will/won't do
## will:
- replace Zalo web
- work in any platform

## won't
- replace Zalo desktop [(there's a guide on installing it on Linux but you try first)](https://sytranvn.dev/posts/zalo-tren-ubuntu/)
- sync your Zalo messages prior to the login date (I can't fix this aoc)
- be mainstream
- get sued or dmcaed by vng. fuck vng
- accept call (voice or video). This used to be available a few months earlier.

# Roadmap
## Phase 1 (COMPLETED)
- Initial release
- Basic modification and other platforms' build

## Phase 2
- Adding support for dark mode and such
- ? who knows?

## To the future
- Allowing the client to sync messages and accept/initiate calls. This depends on how VNG treats the web client. Even the Windows version over Wine can't make or accept call.

# Bugs

- [ ] Right-clicking on an image element in the page to open the menu and select download image or other events does not work (common in MacOS systems). This issue is due to the MacOS built-in webview not supporting this feature.

- [ ] The software currently don't happen to work in Debian (anything newer than trixie) (missing dependencies). On Ubuntu and derriatives it works.

# Shortcuts
<br/>

| Mac                         | Windows/Linux                  | Function                      |
| --------------------------- | ------------------------------ | ----------------------------- |
| <kbd>⌘</kbd> + <kbd>[</kbd> | <kbd>Ctrl</kbd> + <kbd>←</kbd> | Return to the previous page   |
| <kbd>⌘</kbd> + <kbd>]</kbd> | <kbd>Ctrl</kbd> + <kbd>→</kbd> | Go to the next page           |
| <kbd>⌘</kbd> + <kbd>↑</kbd> | <kbd>Ctrl</kbd> + <kbd>↑</kbd> | Auto scroll to top of page    |
| <kbd>⌘</kbd> + <kbd>↓</kbd> | <kbd>Ctrl</kbd> + <kbd>↓</kbd> | Auto scroll to bottom of page |
| <kbd>⌘</kbd> + <kbd>r</kbd> | <kbd>Ctrl</kbd> + <kbd>r</kbd> | Refresh Page                  |
| <kbd>⌘</kbd> + <kbd>w</kbd> | <kbd>Ctrl</kbd> + <kbd>w</kbd> | Hide window, not quite        |
| <kbd>⌘</kbd> + <kbd>-</kbd> | <kbd>Ctrl</kbd> + <kbd>-</kbd> | Zoom out the page             |
| <kbd>⌘</kbd> + <kbd>+</kbd> | <kbd>Ctrl</kbd> + <kbd>+</kbd> | Zoom in the page              |
| <kbd>⌘</kbd> + <kbd>=</kbd> | <kbd>Ctrl</kbd> + <kbd>=</kbd> | Zoom in the Page              |
| <kbd>⌘</kbd> + <kbd>0</kbd> | <kbd>Ctrl</kbd> + <kbd>0</kbd> | Reset the page zoom           |

In addition, double-click the title bar to switch to full-screen mode. For Mac users, you can also use the gesture to go to the previous or next page and drag the title bar to move the window.

</details>

# Compile (for ZaloAlt)
**Pake provides a command line tool, making the flow of package customization quicker and easier. See [documentation](./bin/README.md) for more information.**


# Todo:

0. Rewrite or change documents to fit the project
1. Plugins support. See [Advanced Usage of Pake](https://github.com/tw93/Pake/wiki/Advanced-Usage-of-Pake).

# A thank-you list to be added

# Support me

1. Star this project
2. Give me some ideas to test with
3. Help me build macOS binaries. I don't have any of these devices.
