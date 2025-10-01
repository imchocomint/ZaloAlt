## Installation

Ensure that your Node.js version is 18.0 or higher (e.g., 18.20.2). Avoid using `sudo` for the installation. If you encounter permission issues with npm, refer to [How to fix npm throwing error without sudo](https://stackoverflow.com/questions/16151018/how-to-fix-npm-throwing-error-without-sudo).

```bash
npm install pake-cli -g
```

## Considerations for Windows & Linux Users

- **CRITICAL**: Consult [Tauri prerequisites](https://tauri.app/v1/guides/getting-started/prerequisites) before proceeding.
- For Windows users (ensure that `Win10 SDK (10.0.19041.0)` and `Visual Studio build tool 2022 (>=17.2)` are installed), additional installations are required:

  1. Microsoft Visual C++ 2015-2022 Redistributable (x64)
  2. Microsoft Visual C++ 2015-2022 Redistributable (x86)
  3. Microsoft Visual C++ 2012 Redistributable (x86) (optional)
  4. Microsoft Visual C++ 2013 Redistributable (x86) (optional)
  5. Microsoft Visual C++ 2008 Redistributable (x86) (optional)

- For Ubuntu users, execute the following commands to install the required libraries before compiling:

  ```bash
  sudo apt install libdbus-1-dev \
      libsoup2.4-dev \
      libjavascriptcoregtk-4.0-dev \
      libwebkit2gtk-4.0-dev \
      build-essential \
      curl \
      wget \
      libssl-dev \
      libgtk-3-dev \
      libayatana-appindicator3-dev \
      librsvg2-dev \
      gnome-video-effects \
      gnome-video-effects-extra
  ```

## Usage

### CLI Usage
Prepare your environment before starting. Make sure you have Rust `>=1.63` and Node `>=16` (e.g., `16.18.1`) installed on your computer. For installation guidance, see [Tauri documentation](https://tauri.app/v1/guides/getting-started/prerequisites).

```sh
npm i
npm run dev
npm run build
```
When it says that it can't create a .deb package, do not panic. Go to `$HOME/ZaloAlt/src-tauri/target/release/bundle/deb/`. Find the folder which has the name like this: `zalo-alt_x.y.z_amd64`. Go there and create a Debian package or whatever you want.

## Conclusion

After completing the above steps, your application should be successfully packaged. Please note that the packaging process may take some time depending on your system configuration and network conditions. Be patient, and once the packaging is complete, you can find the application installer in the specified directory.
