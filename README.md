# Cursor Free VIP

A cross-platform utility tool for managing and resetting Cursor editor configuration. Supports Windows, macOS, and Linux.

---

## ✨ Features

- Reset Cursor's local configuration
- Multi-language support: English, 简体中文, 繁體中文, Vietnamese, and more
- Compatible with the latest Cursor versions
- Simple automated setup via script

---

## 💻 System Support

| Operating System | Architecture         | Supported |
|------------------|----------------------|-----------|
| Windows          | x64, x86             | ✅        |
| macOS            | Intel, Apple Silicon | ✅        |
| Linux            | x64, x86, ARM64      | ✅        |

---

## 🚀 Installation

> Run all scripts with administrator / root privileges for best results.  
> Make sure Cursor is fully closed before running.

### Windows (PowerShell as Administrator)

```powershell
irm https://raw.githubusercontent.com/officialumsmcllc/cursor/main/scripts/install.ps1 | iex
```

### Linux / macOS

```bash
curl -fsSL https://raw.githubusercontent.com/officialumsmcllc/cursor/main/scripts/install.sh -o install.sh && chmod +x install.sh && ./install.sh
```

### Arch Linux (AUR)

```bash
yay -S cursor-free-vip-git
```

To stop the script at any time, press `Ctrl+C`.

---

## ⚙️ Configuration

The config file is located at:

```
Windows / macOS / Linux: Documents/.cursor-free-vip/config.ini
```

### Example config.ini

```ini
[Chrome]
chromepath = C:\Program Files\Google\Chrome\Application\chrome.exe

[Turnstile]
handle_turnstile_time = 2
handle_turnstile_random_time = 1-3

[Timing]
min_random_time = 0.1
max_random_time = 0.8
page_load_wait = 0.1-0.8
input_wait = 0.3-0.8
submit_wait = 0.5-1.5
email_check_initial_wait = 4-6
email_refresh_wait = 2-4
max_timeout = 160

[Utils]
check_update = True
show_account_info = True

[WindowsPaths]
storage_path = C:\Users\officialum1\AppData\Roaming\Cursor\User\globalStorage\storage.json
sqlite_path = C:\Users\officialum1\AppData\Roaming\Cursor\User\globalStorage\state.vscdb
machine_id_path = C:\Users\officialum1\AppData\Roaming\Cursor\machineId
cursor_path = C:\Users\officialum1\AppData\Local\Programs\Cursor\resources\app

[OSPaths]
storage_path = /Users/username/Library/Application Support/Cursor/User/globalStorage/storage.json
sqlite_path = /Users/username/Library/Application Support/Cursor/User/globalStorage/state.vscdb
machine_id_path = /Users/username/Library/Application Support/Cursor/machineId
```

---

## 🚨 Common Issues

| Issue | Solution |
|-------|----------|
| Permission denied | Run the script as Administrator (Windows) or with `sudo` (Linux/macOS) |
| Script fails to start | Ensure Cursor is fully closed before running |
| Tool not working after update | Re-run the install script to get the latest version |

---

## 📋 Requirements

- Python 3.8 or higher
- Cursor editor installed
- Administrator / root privileges

---

## 📄 License

This project is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).  
See the [LICENSE](https://github.com/officialumsmcllc/cursor/blob/main/LICENSE.md) file for full details.

---

## ⚠️ Disclaimer

This tool is intended for personal configuration management only.  
Use it responsibly and in accordance with the Cursor editor's terms of service.  
The authors are not responsible for any misuse or consequences arising from use of this tool.
