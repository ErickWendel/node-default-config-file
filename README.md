# Node.js Default Config File Demo 🚀

[![Node.js Version](https://img.shields.io/badge/node.js-v24.1.0+-green.svg)](https://nodejs.org/)
[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)
[![YouTube Video](https://img.shields.io/badge/YouTube-Watch%20Tutorial-red.svg)](https://www.youtube.com/watch?v=ITb0N09KiDU)

This repository demonstrates how to use the **newly added default config file feature** in Node.js v23+. This experimental feature allows you to configure Node.js runtime options using a configuration file instead of command-line flags.

## 📺 YouTube Tutorial

This project is part of my YouTube video tutorial: **[Node.js Default Config File](https://www.youtube.com/watch?v=ITb0N09KiDU)**

## ✨ Features

- 🔧 **Default Configuration**: Use `node.config.json` for runtime options
- 🛠️ **Experimental Flag**: Demonstrates `--experimental-default-config-file`
- 🔍 **Debug Ready**: Pre-configured with inspect and trace-warnings
- 📋 **Schema Validation**: Includes JSON schema for better IDE support

## 📋 Prerequisites

- **Node.js v24.1.0 or higher** (required for the experimental config file feature)

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/ErickWendel/node-default-config-file
   cd node-default-config-file
   ```
2. **Run the application**
   ```bash
   npm start
   ```

## 📁 Project Structure

```
├── index.js           # Main application file
├── node.config.json   # Node.js configuration file
├── package.json       # Project metadata and scripts
├── refs.txt          # Reference links and documentation
└── README.md         # This file
```

## ⚙️ Configuration

The `node.config.json` file contains the Node.js runtime configuration:

```json
{
  "$schema": "https://nodejs.org/dist/v24.1.0/docs/node-config-schema.json",
  "nodeOptions": {
    "inspect": true,
    "trace-warnings": true
  }
}
```

## 🔧 Usage Examples

### Using Default Config File
```bash
# Automatically loads node.config.json
node --experimental-default-config-file index.js
```

### Using Custom Config File
```bash
# Load a specific config file
node --experimental-config-file custom.config.json index.js
```

### With Watch Mode
```bash
# Combine with other Node.js flags
node --experimental-default-config-file --watch index.js
```

## 📚 References

- [Node.js CLI Documentation](https://nodejs.org/api/cli.html)
- [Experimental Default Config File](https://nodejs.org/docs/latest/api/cli.html#--experimental-default-config-file)
- [Node.js Config Schema](https://nodejs.org/dist/v24.0.0/docs/node-config-schema.json)
- [Node.js v23.10.0 Release](https://nodejs.org/en/blog/release/v23.10.0)

## 🎥 Video Tutorial

Watch the complete tutorial on YouTube: [Node.js Default Config File](https://www.youtube.com/watch?v=ITb0N09KiDU)

## 👨‍💻 Author

**Erick Wendel**
- YouTube: [@erickwendel](https://www.youtube.com/@erickwendel)
- Twitter: [@erickwendel_](https://twitter.com/erickwendel_)

## ⚠️ Important Notes

- This feature is **experimental** and may change in future Node.js versions
- Requires Node.js v24.1.0 or higher
- The `--experimental-default-config-file` flag is required to enable this feature

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

---

⭐ **Star this repository** if you found it helpful!

🔔 **Subscribe to my YouTube channel** for more Node.js tutorials! 