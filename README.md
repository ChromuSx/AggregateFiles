# 📂 AggregateFiles Script

## Description
This Python script, called **AggregateFiles**, allows you to copy all files with specific extensions from a source folder and its subfolders into a single destination folder named `FilesAggregate`. This script is particularly useful for those working on projects with many files scattered across different directories, and who want to aggregate relevant files in one place for easier access or analysis. 📁

### Features ✨
- **Included File Extensions**: The script only copies files with specific extensions, including `.sln`, `.csproj`, `.vbproj`, `.cs`, `.html`, `.cshtml`, `.css`, `.js`, `.mrt`, `.json`.
- **Excluded Directories**: Folders such as `.git`, `.vs`, `bin`, `obj`, `Debug`, `Release`, `packages`, `Migrations`, and `SmartAttachments` are excluded from the search, ensuring that only important files are considered.
- **Name Conflict Handling**: If a file with the same name already exists in the destination folder, the new file is renamed by adding a numeric suffix to avoid conflicts.

## How It Works 🛠️
The script performs the following steps:
1. **Creates the destination folder** (`FilesAggregate`) in the same directory as the script if it doesn't already exist.
2. **Scans the source folder and subfolders** to find all files with the specified extensions, ignoring excluded folders.
3. **Copies the files to the destination folder**, handling name conflicts by adding a numeric suffix.

## Requirements 📋
- **Python 3.x**
- Standard Python modules: `os`, `shutil`, `pathlib`

## Usage 🚀
To run the script, simply save it to a Python file (e.g., `AggregateFiles.py`) and execute it:

```sh
python AggregateFiles.py
```

Make sure the script is located in the directory you want to analyze. The script will create a folder named `FilesAggregate` in the same path, where the selected files will be copied.

## Customization 🔧
- **Exclude Directories**: You can modify the `excluded_dirs` list to add or remove directories that you don't want to include in the scan.
- **Included File Extensions**: You can modify the `included_file_extensions` list to add or remove file types to be considered.

## Example Output 🖨️
During execution, the script will print a message for each copied file, for example:
```
Copied: /path/to/source/file.cs -> /path/to/source/FilesAggregate/file.cs
Copied: /path/to/source/file.html -> /path/to/source/FilesAggregate/file_1.html
```

## License 📄
You are free to use and modify this script as needed.
