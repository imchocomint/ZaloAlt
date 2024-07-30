<h1 align="center">ZaloAlt</h1>
<p align="center"><strong>Alternative Zalo client built using <a href="https://www.rust-lang.org/">Rust</a>, <a href="https://tauri.app/">Tauri</a> and <a href="https://github.com/tw93/Pake">Pake</a>.</strong></p>
<div align="center">
    <a href="https://github.com/imchocomint/ZaloAlt/releases" target="_blank">
    <img alt="GitHub downloads" src="https://img.shields.io/github/downloads/imchocomint/ZaloAlt/total.svg?style=flat-square"></a>
</div>

<div align="left"></div>

## Features

- Lighter than the official Zalo app (in term of program size)
- Faster (probably)
- Never take your storage for granted
- Support Linux (hey someone please test it for me)

## Shortcuts
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

## Compile (for ZaloAlt)

![General guide for Pake](https://gw.alipayobjects.com/zos/k/zd/pake.gif)

**Pake provides a command line tool, making the flow of package customization quicker and easier. See [documentation](./bin/README.md) for more information.**

```bash
npm install -g pake-cli
pake chat.zalo.me --name Zalo --icons <path/to/icon.ico>
```

## Development (for Pake only)

Prepare your environment before starting. Make sure you have Rust `>=1.63` and Node `>=16` (e.g., `16.18.1`) installed on your computer. For installation guidance, see [Tauri documentation](https://tauri.app/v1/guides/getting-started/prerequisites).

If you are unfamiliar with these, it is better to try out the above tool to pack with one click.

```sh
# Install Dependencies
npm i

# Local development [Right-click to open debug mode.]
npm run dev

# Pack application
npm run build
```

## Todo:

1. You can refer to the [codebase structure](https://github.com/tw93/Pake/wiki/Description-of-Pake's-code-structure) before working on Pake, which will help you much in development.
2. Modify the `url` and `productName` fields in the `pake.json` file under the src-tauri directory, the "domain" field in the `tauri.config.json` file needs to be modified synchronously, as well as the `icon` and `identifier` fields in the `tauri.xxx.conf.json` file. You can select an `icon` from the `icons` directory or download one from [macOSicons](https://macosicons.com/#/) to match your product needs.
3. For configurations on window properties, you can modify the `pake.json` file to change the value of `width`, `height`, `fullscreen` (or not), `resizable` (or not) of the `windows` property. To adapt to the immersive header on Mac, change `hideTitleBar` to `true`, look for the `Header` element, and add the `padding-top` property.
4. For advanced usages such as style rewriting, advertisement removal, JS injection, container message communication, and user-defined shortcut keys, see [Advanced Usage of Pake](https://github.com/tw93/Pake/wiki/Advanced-Usage-of-Pake).

## A thank-you list to be added



## Frequently Asked Questions

1. Right-clicking on an image element in the page to open the menu and select download image or other events does not work (common in MacOS systems). This issue is due to the MacOS built-in webview not supporting this feature.

## Support Pake, the base of the project

1. I have two cats, TangYuan and Coke. If you think Pake delights your life, you can feed them <a href="https://miaoyan.app/cats.html?name=Pake" target="_blank">some canned food 🥩</a>.
2. If you like Pake, you can star it on GitHub. Also, welcome to [recommend Pake](https://twitter.com/intent/tweet?url=https://github.com/tw93/Pake&text=%23Pake%20-%20A%20simple%20Rust%20packaged%20web%20pages%20to%20generate%20Mac%20App%20tool,%20compared%20to%20traditional%20Electron%20package,%20the%20size%20of%20nearly%2040%20times%20smaller,%20generally%20about%202M,%20the%20underlying%20use%20of%20Tauri,%20performance%20experience%20than%20the%20JS%20framework%20is%20much%20lighter~) to your friends.
3. You can follow my [Twitter](https://twitter.com/HiTw93) to get the latest news of Pake or join our [Telegram](https://t.me/+GclQS9ZnxyI2ODQ1) chat group.
4. I hope that you enjoy playing with it. Let us know if you find a website that would be great for a Mac App!

## Support me

1. Star this project
2. Give me some ideas to test with
3. Help me to build Linux and macOS binaries. I don't have any of these devices.
