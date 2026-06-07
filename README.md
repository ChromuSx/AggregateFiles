# 📂 AggregateFiles

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/license-MIT-green.svg?style=for-the-badge" alt="MIT License">
  <img src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-blue?style=for-the-badge" alt="Platform">
</div>

<p align="center">
  <a href="https://github.com/sponsors/ChromuSx"><img src="https://img.shields.io/badge/Sponsor-GitHub-EA4AAA?style=for-the-badge&logo=github-sponsors&logoColor=white" alt="GitHub Sponsors"></a>
  <a href="https://ko-fi.com/chromus"><img src="https://img.shields.io/badge/Support-Ko--fi-FF5E5B?style=for-the-badge&logo=ko-fi&logoColor=white" alt="Ko-fi"></a>
  <a href="https://buymeacoffee.com/chromus"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me a Coffee"></a>
  <a href="https://www.paypal.com/paypalme/giovanniguarino1999"><img src="https://img.shields.io/badge/Donate-PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white" alt="PayPal"></a>
</p>

<p align="center">
  <strong>Python script that aggregates all files with specific extensions from a directory tree into a single folder — perfect for feeding an entire project to an AI or code analysis tool.</strong>
</p>

## ✨ Features

- **Targeted extensions**: copies only `.sln`, `.csproj`, `.cs`, `.html`, `.cshtml`, `.css`, `.js`, `.json` and more
- **Smart exclusions**: skips `.git`, `bin`, `obj`, `node_modules`, `Migrations` and other noise folders automatically
- **Conflict handling**: renames duplicates with a numeric suffix — no overwrites
- **Zero dependencies**: uses only Python standard library (`os`, `shutil`, `pathlib`)

## 📋 Requirements

- Python 3.x

## 🚀 Usage

Place the script in the root of the directory you want to scan, then run:

```bash
python AggregateFiles.py
```

A `FilesAggregate/` folder will be created in the same location with all matching files collected.

## ⚙️ Customization

Edit these two lists at the top of the script:

```python
excluded_dirs = [".git", ".vs", "bin", "obj", "Debug", "Release", "packages", "Migrations"]
included_file_extensions = [".sln", ".csproj", ".cs", ".html", ".cshtml", ".css", ".js", ".json"]
```

## 📄 License

MIT — see [LICENSE](LICENSE).

<div align="center">
  <strong>Made with ❤️ by <a href="https://github.com/ChromuSx">Giovanni Guarino</a></strong>
</div>
