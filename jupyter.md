# 🚀 Jupyter Notebook Cheatsheet

## 🎯 Essential Modes
| Mode | Border Color | Description |
|------|-------------|-------------|
| **Command Mode** | Blue | Navigate & manipulate cells |
| **Edit Mode** | Green | Edit cell content |

**Switch modes:**
- `Esc` → Command mode
- `Enter` → Edit mode

---

## ⚡ Must-Know Shortcuts

### ▶️ Running Cells
| Shortcut | Action |
|----------|--------|
| `Shift + Enter` | Run cell, select next |
| `Ctrl + Enter` | Run cell, stay selected |
| `Alt + Enter` | Run cell, insert new below |

### 📝 Cell Creation & Deletion
| Shortcut | Action |
|----------|--------|
| `A` | Insert cell **above** |
| `B` | Insert cell **below** |
| `DD` | **Delete** cell (press D twice) |
| `Z` | **Undo** delete |

### 🔄 Cell Types
| Shortcut | Action |
|----------|--------|
| `Y` | Change to **Code** |
| `M` | Change to **Markdown** |
| `R` | Change to **Raw** |

### 📋 Copy/Paste/Move
| Shortcut | Action |
|----------|--------|
| `C` | **Copy** cell |
| `X` | **Cut** cell |
| `V` | **Paste** cell below |
| `Shift + V` | **Paste** cell above |

### ⬆️⬇️ Moving Cells
| Shortcut | Action |
|----------|--------|
| `Ctrl + Shift + ↑` | Move cell(s) **up** |
| `Ctrl + Shift + ↓` | Move cell(s) **down** |

---

## 🎯 Navigation Shortcuts

### 🏃 Quick Movement
| Shortcut | Action |
|----------|--------|
| `↑` / `↓` | Move between cells |
| `Ctrl + Home` | Go to **first** cell |
| `Ctrl + End` | Go to **last** cell |
| `Shift + ↑/↓` | **Select multiple** cells |

### 🔍 Finding & Replacing
| Shortcut | Action |
|----------|--------|
| `Ctrl + F` | **Find** in current cell |
| `Ctrl + H` | **Find & Replace** |
| `Ctrl + G` | Go to line number |

---

## 💻 Code Editing (Edit Mode)

### ✨ Smart Editing
| Shortcut | Action |
|----------|--------|
| `Tab` | **Code completion** / Indent |
| `Shift + Tab` | **Tooltip/Help** |
| `Ctrl + ]` | **Indent** |
| `Ctrl + [` | **Unindent** |
| `Ctrl + /` | **Comment/Uncomment** |
| `Ctrl + D` | **Delete line** |

### 🎯 Advanced Editing
| Shortcut | Action |
|----------|--------|
| `Ctrl + A` | Select **all** in cell |
| `Ctrl + Z` | **Undo** |
| `Ctrl + Y` | **Redo** |
| `Ctrl + Shift + -` | **Split** cell at cursor |

---

## 🛠️ Kernel & System

### 🔄 Kernel Control
| Shortcut | Action |
|----------|--------|
| `00` | **Restart** kernel (press 0 twice) |
| `Ctrl + C` | **Interrupt** kernel |
| `Shift + L` | Toggle **line numbers** |
| `Shift + O` | Toggle **output scrolling** |

### 💾 Save & Export
| Shortcut | Action |
|----------|--------|
| `Ctrl + S` | **Save** notebook |
| `Ctrl + Shift + S` | **Save As** |

---

## 🧙 Advanced Tips

### 🎯 Multi-Selection
- `Ctrl + Click` → Select multiple non-adjacent cells
- `Shift + Click` → Select range of cells
- Selected cells can be moved/deleted together

### 🚀 Magic Commands
```python
%time          # Time single execution
%%time         # Time entire cell
%who           # Show variables
%history       # Show command history
%matplotlib inline  # Inline plots
!ls            # Run shell commands
```

### 🎨 Markdown Quick Reference
```markdown
# Header 1
## Header 2
**bold** *italic*
`code`
- bullet points
1. numbered lists
[link](url)
![image](path)
```

### 🔧 Useful Cell Magics
```python
%%bash         # Run cell as bash
%%html         # Render as HTML  
%%javascript   # Run JavaScript
%%latex        # Render LaTeX
%%writefile filename.py  # Save cell to file
```

---

## 🆘 Emergency Shortcuts

| Problem | Solution |
|---------|----------|
| **Stuck in long execution** | `Ctrl + C` (interrupt) |
| **Notebook frozen** | `00` (restart kernel) |
| **Accidentally deleted cell** | `Z` (undo) |
| **Lost in large notebook** | `Ctrl + Home/End` |
| **Can't see output** | `Shift + O` (toggle scroll) |

---

## 💡 Pro Productivity Tips

1. **Use `Shift + Tab`** for instant documentation
2. **Master `A` and `B`** for quick cell insertion
3. **`DD` is faster** than clicking delete
4. **Select multiple cells** for batch operations
5. **Toggle line numbers** with `Shift + L` for debugging
6. **Use magic commands** for system operations
7. **`Ctrl + Shift + -`** to split long cells
8. **Learn the `%%` cell magics** for special cell types

---

*💡 Remember: Most shortcuts work in **Command Mode** (blue border). Press `Esc` first!*