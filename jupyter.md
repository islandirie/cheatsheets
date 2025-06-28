# Jupyter Lab - Essential Cheat Sheet

## 🎯 Two Modes
- **Command Mode** (blue border): Navigate and manipulate notebook structure
- **Edit Mode** (green border): Edit cell content

---

## ⌨️ Most Important Shortcuts

### Mode Switching
| Shortcut | Action |
|----------|--------|
| `Enter` | Enter Edit mode |
| `Esc` | Enter Command mode |

### Essential Navigation
| Shortcut | Action |
|----------|--------|
| `↑/↓` | Navigate cells (Command mode) |
| `Shift + Enter` | Run cell and move to next |
| `Ctrl + Enter` | Run cell and stay in place |
| `Alt + Enter` | Run cell and insert new below |

### Cell Operations (Command Mode)
| Shortcut | Action |
|----------|--------|
| `A` | Insert cell above |
| `B` | Insert cell below |
| `DD` | Delete cell (press D twice) |
| `Z` | Undo cell deletion |
| `C` | Copy cell |
| `V` | Paste cell below |
| `X` | Cut cell |

### Cell Types (Command Mode)
| Shortcut | Action |
|----------|--------|
| `Y` | Change to Code cell |
| `M` | Change to Markdown cell |
| `R` | Change to Raw cell |

### Running Code
| Shortcut | Action |
|----------|--------|
| `Shift + Enter` | Run cell, select next |
| `Ctrl + Enter` | Run cell |
| `Alt + Enter` | Run cell, insert below |
| `Ctrl + Shift + Enter` | Run all cells |

---

## 🔧 File and Notebook Operations

### File Menu Shortcuts
| Shortcut | Action |
|----------|--------|
| `Ctrl + S` | Save notebook |
| `Ctrl + Shift + S` | Save As |
| `Ctrl + O` | Open file |
| `Ctrl + N` | New notebook |

### Kernel Operations
| Shortcut | Action |
|----------|--------|
| `0 0` | Restart kernel (press 0 twice) |
| `I I` | Interrupt kernel (press I twice) |

---

## ✏️ Edit Mode Shortcuts

### Basic Editing
| Shortcut | Action |
|----------|--------|
| `Tab` | Code completion or indent |
| `Shift + Tab` | Show function tooltip |
| `Ctrl + ]` | Indent |
| `Ctrl + [` | Dedent |
| `Ctrl + A` | Select all |
| `Ctrl + Z` | Undo |
| `Ctrl + Y` | Redo |

### Advanced Editing
| Shortcut | Action |
|----------|--------|
| `Ctrl + /` | Comment/uncomment |
| `Ctrl + D` | Delete line |
| `Ctrl + Shift + K` | Delete line |
| `Alt + Click` | Multi-cursor |
| `Ctrl + F` | Find and replace |

---

## 🎨 Markdown Cells Quick Reference

### Headers
```markdown
# H1 Header
## H2 Header
### H3 Header
#### H4 Header
```

### Text Formatting
```markdown
**Bold text**
*Italic text*
***Bold and italic***
`inline code`
~~Strikethrough~~
```

### Lists
```markdown
- Bullet point
- Another point
  - Nested point

1. Numbered list
2. Second item
   1. Nested numbered
```

### Code Blocks
````markdown
```python
def hello():
    print("Hello World!")
```
````

### Links and Images
```markdown
[Link text](https://example.com)
![Alt text](image.jpg)
```

### Math (LaTeX)
```markdown
Inline math: $E = mc^2$
Block math: $$\int_0^\infty e^{-x^2} dx$$
```

---

## 🎯 Command Palette & Advanced

### Command Palette
| Shortcut | Action |
|----------|--------|
| `Ctrl + Shift + C` | Open command palette |

### Common Commands
- Type in command palette:
  - "split" - Split cell at cursor
  - "merge" - Merge selected cells
  - "clear" - Clear cell output
  - "restart" - Restart kernel
  - "export" - Export notebook

### Useful Magic Commands

#### Cell Magics (start with %%)
```python
%%time          # Time cell execution
%%timeit        # Benchmark cell multiple times
%%writefile     # Write cell content to file
%%bash          # Run bash commands
%%html          # Render as HTML
```

#### Line Magics (start with %)
```python
%pwd            # Current directory
%ls             # List files
%cd             # Change directory
%who            # List variables
%whos           # List variables with details
%matplotlib inline  # Enable inline plots
%load           # Load code from file
%run            # Run Python script
%reset          # Clear all variables
```

---

## 🚀 Pro Tips

### Productivity Hacks
1. **Quick Help**: `Shift + Tab` shows function documentation
2. **Autocomplete**: `Tab` for code completion
3. **Multi-line Selection**: Hold `Alt` and click to place multiple cursors
4. **Cell Folding**: Click the blue bar on the left of cells
5. **Output Scrolling**: Right-click output → "Enable Scrolling for Outputs"

### Variable Inspection
```python
# Quick variable inspection
?variable_name          # Basic info
??variable_name         # Source code
variable_name?          # Same as ?variable_name
```

### Debugging
```python
%debug                  # Debug after exception
%pdb                    # Auto-debug on exception
import pdb; pdb.set_trace()  # Breakpoint
```

### Memory & Performance
```python
%memit expression       # Memory usage
%lprun -f func func()   # Line profiler
%load_ext memory_profiler  # Load memory profiler
```

---

## 💡 Quick Reference Summary

**Most Used Daily:**
- `Shift + Enter` - Run and advance
- `B` - New cell below
- `DD` - Delete cell
- `M/Y` - Markdown/Code mode
- `Ctrl + S` - Save

**For Efficiency:**
- `Tab` - Autocomplete
- `Shift + Tab` - Documentation
- `Ctrl + Shift + C` - Command palette
- `%%time` - Time execution
- `%who` - List variables

**Remember First**:
Shift+Enter (run and advance)
B (new cell Below)
DD (delete cell)
M/Y (switch to Markdown/Code)
Tab (autocomplete)
Shift + Tab (show documentation)
