<div align="center">

<img src="docs/assets/logo.png" alt="Prism Logo" width="128" />

# Prism

**A modern, beautiful Windows system cleaner & optimizer**

Built with [Tauri v2](https://tauri.app/) + [React](https://react.dev/) + [Fluent UI](https://react.fluentui.dev/)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Platform: Windows](https://img.shields.io/badge/Platform-Windows-0078D6?logo=windows)
![Built with Tauri](https://img.shields.io/badge/Tauri-v2-FFC131?logo=tauri)

[繁體中文](README.zh-TW.md) | [简体中文](README.zh-CN.md)

<img src="docs/screenshots/01-dashboard.png" alt="Dashboard" width="720" />

</div>

---

## ✨ Features

| Module | Description |
|--------|-------------|
| 📊 **Dashboard** | Real-time system overview — CPU, memory, disk, network with health score |
| 🧹 **Deep Clean** | Scan and remove browser cache, temp files, logs, and app leftovers |
| 📦 **Uninstaller** | Smart app removal with size sorting and batch uninstall |
| ⚡ **Optimizer** | Flush DNS, rebuild icon/font/thumbnail caches |
| 💽 **Disk Analysis** | Interactive donut chart visualization of disk usage |
| 📈 **Monitor** | Live CPU/Memory/Disk charts with 2-second refresh |
| 🗑️ **Build Cleanup** | Purge `node_modules`, `.gradle`, `target`, `__pycache__` and more |
| 🌐 **i18n** | English, 繁體中文, 简体中文 — auto-detects system language |

## 🖼️ Screenshots

<details>
<summary>Click to expand all screenshots</summary>

| Feature | Screenshot |
|---------|-----------|
| Deep Clean | <img src="docs/screenshots/02-deep-clean.png" width="600" /> |
| Uninstaller | <img src="docs/screenshots/03-uninstaller.png" width="600" /> |
| Optimizer | <img src="docs/screenshots/04-optimizer.png" width="600" /> |
| Disk Analysis | <img src="docs/screenshots/05-disk-analysis.png" width="600" /> |
| Monitoring | <img src="docs/screenshots/06-monitoring.png" width="600" /> |
| Build Cleanup | <img src="docs/screenshots/07-build-cleanup.png" width="600" /> |
| Settings | <img src="docs/screenshots/08-settings.png" width="600" /> |

</details>

## 🚀 Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) 18+
- [Rust](https://www.rust-lang.org/tools/install) (stable)
- [Tauri CLI prerequisites](https://v2.tauri.app/start/prerequisites/)

### Development

```bash
# Clone the repository
git clone https://github.com/YourUsername/prism.git
cd prism

# Install dependencies
npm install

# Start dev server
npm run tauri dev
```

### Build

```bash
# Build production installer
npm run tauri build
```

The installer will be output to `src-tauri/target/release/bundle/`.

## 🏗️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18 + TypeScript + Vite |
| UI Components | Fluent UI React v9 |
| Backend | Rust + Tauri v2 |
| Core Engine | PowerShell scripts |
| i18n | react-i18next |
| Styling | Custom CSS (glassmorphism) |

## 📁 Project Structure

```
prism/
├── src/                    # React frontend
│   ├── components/         # Reusable UI components
│   ├── pages/              # Page components
│   ├── hooks/              # Custom React hooks
│   ├── i18n/               # Internationalization
│   │   ├── i18n.ts         # i18next configuration
│   │   └── locales/        # Translation files (en, zh-TW, zh-CN)
│   ├── App.tsx             # Root component
│   └── main.tsx            # Entry point
├── src-tauri/              # Rust backend
│   ├── src/
│   │   ├── commands/       # Tauri command handlers
│   │   └── lib.rs          # Plugin registration
│   ├── Cargo.toml
│   └── tauri.conf.json
├── mole-core/              # PowerShell core scripts
└── package.json
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🙏 Acknowledgements

- **[Mole](https://github.com/nicholasgasior/mole)** by [tw93](https://github.com/tw93) — the open-source PowerShell core engine that powers Prism's cleaning and optimization features (MIT License)
- **[Tauri](https://tauri.app/)** — the framework for building lightweight, secure desktop apps
- **[Fluent UI](https://react.fluentui.dev/)** — Microsoft's design system for React
- **[react-i18next](https://react.i18next.com/)** — internationalization framework

See [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) for the full list of dependencies and their licenses.

---

## Support

If this project saved you some time, you can [buy me a coffee](https://buymeacoffee.com/iml1s).

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
