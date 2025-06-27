# PowerShell Basics

This cheat sheet covers the most common PowerShell commands used for file navigation, directory management, and basic scripting tasks.

---

## Directory Navigation

| Command         | Description                                         |
|-----------------|-----------------------------------------------------|
| `dir`           | Lists all folders and files in the current path     |
| `cd`            | Changes the current directory to a given path       |
| `cd /`          | Moves to the root directory                         |
| `cd ..`         | Moves up one level in the directory tree            |
| `cd ../..`      | Moves up two levels                                 |
| `pwd`           | Displays the current working directory              |

---

## File and Folder Management

| Command                   | Description                                 |
|---------------------------|---------------------------------------------|
| `mkdir FolderName`        | Creates a new folder                        |
| `rmdir FolderName`        | Deletes a folder (if empty)                 |
| `del FileName`            | Deletes a file                              |
| `New-Item FileName`       | Creates a new file                          |
| `copy Item1 Item2`        | Copies a file or folder                     |
| `move Item1 Item2`        | Moves or renames a file/folder              |

---

## Viewing and Editing Files

| Command                        | Description                             |
|--------------------------------|-----------------------------------------|
| `type FileName`                | Displays contents of a text file        |
| `notepad FileName`             | Opens a file in Notepad                 |
| `code FileName`                | Opens a file in Visual Studio Code      |

> If `code` doesn't work, ensure VS Code CLI is installed:  
> Open VS Code → Press `Ctrl+Shift+P` → Type: *Shell Command: Install 'code' command in PATH*

---

## Script Execution (Optional)

| Command                            | Description                                    |
|------------------------------------|------------------------------------------------|
| `.\script.ps1`                     | Runs a PowerShell script in the current folder |
| `Set-ExecutionPolicy RemoteSigned` | Allows scripts to run (use with care)          |

---

## Notes

- PowerShell is case-insensitive, but file and folder names may be case-sensitive depending on the environment.
- Use `Tab` to auto-complete paths and file names.
- Use `cls` to clear the terminal screen.

---

For more advanced PowerShell help, type: Get-Help or Get-Command