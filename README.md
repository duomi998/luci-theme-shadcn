<h4 align="right"><strong>English</strong> | <a href="README_zh.md">简体中文</a></h4>
<p align="center">
    <img src="https://raw.githubusercontent.com/eamonxg/assets/master/shadcn/logo/logo.svg" width="96"/>
</p>
<h1 align="center">Shadcn LuCI Theme</h1>
<p align="center"><strong>A modern sidebar LuCI theme for OpenWrt, built with shadcn/ui design language.</strong></p>
<h4 align="center">🗂️ Sidebar Layout | 🌗 Dark / Light Mode | 📱 Mobile Drawer | 🎨 OKLCH Tokens</h4>
<div align="center">
  <a href="https://openwrt.org"><img alt="OpenWrt" src="https://img.shields.io/badge/OpenWrt-%E2%89%A523.05-00B5E2?logo=openwrt&logoColor=white"></a>
  <a href="https://www.google.com/chrome/"><img alt="Chrome" src="https://img.shields.io/badge/Chrome-%E2%89%A5111-4285F4?logo=googlechrome&logoColor=white"></a>
  <a href="https://www.apple.com/safari/"><img alt="Safari" src="https://img.shields.io/badge/Safari-%E2%89%A516.4-000000?logo=safari&logoColor=white"></a>
  <a href="https://www.mozilla.org/firefox/"><img alt="Firefox" src="https://img.shields.io/badge/Firefox-%E2%89%A5128-FF7139?logo=firefoxbrowser&logoColor=white"></a>
  <a href="https://github.com/eamonxg/luci-theme-shadcn/releases/latest"><img alt="GitHub release" src="https://img.shields.io/github/v/release/eamonxg/luci-theme-shadcn"></a>
  <a href="https://github.com/eamonxg/luci-theme-shadcn/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/eamonxg/luci-theme-shadcn/total"></a>
</div>

<div align="center">
  <img src="https://raw.githubusercontent.com/eamonxg/assets/master/shadcn/preview/overview.png" alt="Overview" width="100%">
</div>

## Features

- **Sidebar layout**: Collapsible sidebar with accordion sub-menus and mobile drawer.
- **Dark / Light mode**: Built-in toggle, preference persisted via `localStorage`, flash-free restore on load.
- **shadcn/ui design**: Semantic color tokens, `rounded-lg` components, `hover:bg-muted` interactions.
- **OKLCH color system**: All colors defined as OKLCH custom properties — easy to theme.
- **Modern stack**: Vite + TailwindCSS v4 build, Inter variable font, Lucide icons.

## Preview

<div align="center">
  <img src="https://raw.githubusercontent.com/eamonxg/assets/master/shadcn/preview/login.png" alt="Login Page" width="49%">
  <img src="https://raw.githubusercontent.com/eamonxg/assets/master/shadcn/preview/mobile.png" alt="Mobile View" width="49%">
</div>

## Compatibility

- **OpenWrt**: Requires OpenWrt 23.05.0 or later (ucode templates + LuCI JavaScript APIs).
- **Browsers**: Built with TailwindCSS v4, requires:
  - **Chrome/Edge 111+** _(March 2023)_
  - **Safari 16.4+** _(March 2023)_
  - **Firefox 128+** _(July 2024)_

## Installation

OpenWrt 25.12+ and snapshots use `apk`; older versions use `opkg`.

> **Tip**: Run `opkg --version` or `apk --version` to check which package manager your device has.

- **opkg** (OpenWrt < 25.12):

  ```sh
  cd /tmp && uclient-fetch -O luci-theme-shadcn.ipk https://github.com/eamonxg/luci-theme-shadcn/releases/latest/download/luci-theme-shadcn_0.1.0-r20260520_all.ipk && opkg install luci-theme-shadcn.ipk
  ```

- **apk** (OpenWrt 25.12+ and snapshots):

  ```sh
  cd /tmp && uclient-fetch -O luci-theme-shadcn.apk https://github.com/eamonxg/luci-theme-shadcn/releases/latest/download/luci-theme-shadcn-0.1.0-r20260520.apk && apk add --allow-untrusted luci-theme-shadcn.apk
  ```

## License & Acknowledgments

[Apache 2.0](LICENSE). Thanks to:

- [shadcn/ui](https://github.com/shadcn-ui/ui) — component aesthetics, tokens, and interaction patterns
- [Lucide](https://github.com/lucide-icons/lucide) — icons
- [Linear](https://linear.app) — layout and typography inspiration
- [Vite](https://vite.dev/) and [Tailwind CSS](https://tailwindcss.com/)
- [luci-theme-bootstrap](https://github.com/openwrt/luci/tree/master/themes/luci-theme-bootstrap) — template structure and LuCI integration patterns
- [Claude Code](https://claude.ai/code)
