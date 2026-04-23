# HIDERZ v1.0 — Folder Hider & Locker

> A lightweight Windows batch script that hides and locks folders with a password — no installations, no admin rights, pure `.bat` magic.

---

## Features

- **Lock & Hide Any Folder** — instantly hides your folder and makes it inaccessible
- **Password-Protected Access** — only the correct password reveals the folder
- **System Attribute Cloaking** — uses `+s +h` flags to hide from Windows Explorer
- **Zero Dependencies** — no installs, no admin rights, no external tools
- **Easy to Use** — set your password once, lock and unlock anytime

---

## Requirements

- Windows 10 or 11
- Basic file system permissions
- CMD or PowerShell

---

## Getting Started

### 1. Download or clone the repo

```bash
git clone https://github.com/Finnapple/HIDERZ.git
cd HIDERZ
```

### 2. Set your password

Open `HIDERZ.bat` in any text editor and find this line:

```bat
if "%pass%" NEQ "your password here" goto FAIL
```

Replace `your password here` with your desired password, then save the file.

### 3. Run the script

Double-click `HIDERZ.bat` or run it from CMD:

```bash
HIDERZ.bat
```

---

## How It Works

| Action | What to Do |
|---|---|
| **First Run** | Creates a folder named `Private` if it doesn't exist |
| **Lock Folder** | Run script while `Private` exists → Press `Y` to hide & lock it |
| **Unlock Folder** | Run script again → Enter correct password → Folder is restored |
| **Cancel** | Press `N` or close the window at any prompt |

---

## Use Cases

- Hide sensitive files on shared or public PCs
- Temporarily protect project folders or personal documents
- Quick, script-based privacy without third-party apps

---

## Disclaimer

HIDERZ uses Windows folder hiding techniques — **not encryption**. It is intended for **basic local privacy**, not high-security purposes. Anyone familiar with batch scripting or Windows internals may be able to bypass it. Use responsibly and do not rely on it for sensitive or critical data.

---

## License

MIT License © 2025 Finnapple

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

<p align="center">Made by <a href="https://github.com/Finnapple">Finnapple</a> — suggestions and forks welcome!</p>
