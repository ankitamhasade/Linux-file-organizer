# Linux File Organizer and Backup Tool

A simple Bash script that backs up a folder and then sorts its files into
`Images`, `Documents`, `Videos` and `Others` based on file extension.

## Features
- Creates a compressed backup (`.tar.gz`) with date and time before changing anything
- Sorts files by extension using a `case` statement
- Works on any folder you pass as an argument (default: `~/Downloads`)
- Prints a short summary when finished

## Usage
```bash
chmod +x file_organizer.sh
./file_organizer.sh ~/Downloads
```
Backups are saved in `~/backups/`.

## Example
Before:
```
a.jpg  b.pdf  c.mp4  d.zip
```
After:
```
Images/a.jpg   Documents/b.pdf   Videos/c.mp4   Others/d.zip
```
## Linux commands and concepts used
`mkdir -p`, `tar -czf`, `date`, `mv`, `for` loop, `case` statement,
command-line arguments, brace expansion

## Possible improvements
- Handle duplicate file names
- Save a log file of moved files
- Run automatically with `cron`

## Author
Ankita Mhasade
