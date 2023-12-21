# Vim Cheatsheet for Basic Editing
### Notes
- In command line (mac) type VimTutor to learn Vim.
    - Learning Checkpoint, Lesson 4.1: CURSOR LOCATION AND FILE STATUS
- format for a change command is:
    operator \[number\] command
- operator - what to do, such as d for delete
- \[number\] - count to repeat motion
- motion - moves over the text

## Moving Around:
- `h` - Move left
- `j` - Move down
- `k` - Move up
- `l` - Move right
- `w` - Move to the beginning of the next word
- `e` - Move to the end of the next word
- `b` - Move to the beginning of the previous word
- `0` - Move to the beginning of the line
- `$` - Move to the end of the line
- `gg` - Go to the beginning of the document
- `G` - Go to the end of the document
- `:line_number` - Move to a specific line

## Editing:
- `i` - Enter insert mode before the cursor
- `I` - Enter insert mode at the beginning of the line
- `a` - Enter append mode after the cursor
- `A` - Enter Append mode at the end of the line
- `o` - Open a new line below the current line and enter insert mode
- `O` - Open a new line above the current line and enter insert mode
- `dd` - Delete the current line
- `dw` - Delete from the cursor to the beginning of the next word
- `cw` - Change from the cursor to the beginning of the next word
- `ce` - Change from the cursor to the end of the word
- `cc` - Change the whole line
- `r[x]` - Replace character with any typed character
- `x` - Delete the character under the cursor

## Exiting and Saving:
- `:w` - Save changes
- `:q` - Quit (close) Vim
- `:wq` - Save changes and quit
- [`:q!`](#) - Quit without saving (force quit)

## Searching and Replacing:
- `/pattern` - Search for a pattern
- `n` - Move to the next search result
- `N` - Move to the previous search result
- `:s/old/new/g` - Replace all occurrences of "old" with "new" in the current line
- `:%s/old/new/g` - Replace all occurrences of "old" with "new" in the entire document

## Visual Mode:
- `v` - Enter visual mode to select text
- `V` - Enter visual line mode (select whole lines)
- `Ctrl` + `v` - Enter visual block mode (select a block of text)

## Copy and Paste:
- `y` - Yank (copy) selected text
- `p` - Paste after the cursor
- `P` - Paste before the cursor

## Other Useful Commands:
- `u` - Undo
- `Ctrl` + `r` - Redo
- `.` - Repeat the last command
