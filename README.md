# pscol

`pscol` is a small utility for the **Bash shell** that lets you quickly change the color of your `user@host` prompt.

## Why it exists

If you SSH into multiple servers, or virtual machines, it’s easy to forget where you are.  
`pscol` helps by giving each system a distinct prompt color. Much like having a red notebook for work notes, and a blue notebook for personal notes.

**For example, one could do:**
Red = production  
Green = development or testing  
Blue = personal desktop \ laptop  

## What it does

- Changes only the `user@host` color in your Bash prompt  
- Leaves the rest of the prompt (like your current directory) unchanged  
- Works best on systems that use a Debian-style colored prompt (Debian, Ubuntu, Fedora)  
- Creates a backup of your `~/.bashrc` before modifying it  

## Requirements

- Bash shell  
- Standard GNU tools (`grep`, `awk`, `sed`, etc.)

## Notes

- Assumes your prompt is already colorized (like Debian defaults)  
- On systems with a plain prompt (e.g. void and some others), it may overwrite your existing `PS1`
- Written to operate on **.bashrc** so it isn't going to work as-is on other shell configs.

## Usage

```bash
./pscol
