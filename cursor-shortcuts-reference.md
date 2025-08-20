# Cursor IDE Keyboard Shortcuts Reference

*A comprehensive guide to Cursor IDE shortcuts for Mac and Windows*

Based on research from [Cursor101](https://cursor101.com/cursor/cheat-sheet), [Starmorph Blog](https://blog.starmorph.com/blog/vs-code-mac-keyboard-shortcuts-guide-for-developers), and [Mehmet Baykar](https://www.mehmetbaykar.com/posts/top-15-cursor-shortcuts-to-speed-up-development/).

---

## 🤖 Cursor AI-Specific Features

### Essential AI Shortcuts
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Open Chat | `⌘L` | `Ctrl+L` | Open AI chat interface |
| Open Composer | `⌘I` | `Ctrl+I` | Open Cursor Composer (floating window) |
| Open Full-screen Composer | `⌘⇧I` | `Ctrl+Shift+I` | Open Composer in full-screen mode |
| Inline Editing (Cmd K) | `⌘K` | `Ctrl+K` | Open inline AI editing |
| Toggle Agent in Composer | `⌘.` | `Ctrl+.` | Switch between AI agents |
| Toggle between AI models | `⌘/` | `Ctrl+/` | Switch AI models |

### AI Code Completion (Cursor Tab)
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Accept Suggestion | `Tab` | `Tab` | Accept AI code suggestion |
| Reject Suggestion | `Esc` | `Esc` | Reject AI suggestion |
| Partial Accept | `⌘→` | `Ctrl+→` | Accept next word of suggestion |

### AI Context & References
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Add selection to Chat | `⌘⇧L` | `Ctrl+Shift+L` | Add selected code to chat |
| Add selection to Edit | `⌘⇧K` | `Ctrl+Shift+K` | Add selected code to edit |
| Submit with codebase | `⌘Enter` | `Ctrl+Enter` | Send message with full codebase context |

### AI Inline Editing
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Apply Changes | `⌘Enter` | `Ctrl+Enter` | Apply AI suggested changes |
| Cancel/Delete Changes | `⌘Backspace` | `Ctrl+Backspace` | Cancel AI changes |

### AI @ Symbols (Context References)
| Symbol | Usage | Description |
|--------|-------|-------------|
| `@filename` | `@package.json` | Reference specific file |
| `@functionName` | `@handleSubmit` | Reference specific function |
| `@variableName` | `@userState` | Reference specific variable |
| `@codebase` | `@codebase query` | Search entire codebase |
| `@web` | `@web latest React patterns` | Search web for information |

---

## 📂 General IDE Operations

### Command Palette & Settings
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Show Command Palette | `⌘⇧P` or `F1` | `Ctrl+Shift+P` or `F1` | Open command palette |
| Quick Open (Go to File) | `⌘P` | `Ctrl+P` | Quick file search |
| User Settings | `⌘,` | `Ctrl+,` | Open settings |
| Keyboard Shortcuts | `⌘K ⌘S` | `Ctrl+K Ctrl+S` | Open keyboard shortcuts |
| Cursor Settings | `⌘⇧J` | `Ctrl+Shift+J` | Open Cursor-specific settings |

### Window Management
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| New window/instance | `⇧⌘N` | `Ctrl+Shift+N` | Create new window |
| Close window/instance | `⌘W` | `Ctrl+W` | Close current window |
| Toggle full screen | `⌃⌘F` | `F11` | Toggle fullscreen mode |
| Zen Mode | `⌘K Z` | `Ctrl+K Z` | Enter zen mode (Esc Esc to exit) |

---

## ✏️ Basic Editing

### Line Operations
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Cut line | `⌘X` | `Ctrl+X` | Cut current line |
| Copy line | `⌘C` | `Ctrl+C` | Copy current line |
| Delete line | `⇧⌘K` | `Ctrl+Shift+K` | Delete entire line |
| Insert line below | `⌘Enter` | `Ctrl+Enter` | Insert new line below |
| Insert line above | `⇧⌘Enter` | `Ctrl+Shift+Enter` | Insert new line above |
| Move line up/down | `⌥↑/⌥↓` | `Alt+↑/Alt+↓` | Move line up or down |
| Copy line up/down | `⇧⌥↑/⇧⌥↓` | `Shift+Alt+↑/Shift+Alt+↓` | Duplicate line up or down |

### Text Navigation
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Go to beginning/end of line | `Home/End` | `Home/End` | Navigate to line start/end |
| Go to beginning/end of file | `⌘↑/⌘↓` | `Ctrl+Home/Ctrl+End` | Navigate to file start/end |
| Jump to matching bracket | `⇧⌘\` | `Ctrl+Shift+\` | Jump to matching bracket |

### Indentation & Formatting
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Indent/outdent line | `⌘]/⌘[` | `Ctrl+]/Ctrl+[` | Increase/decrease indentation |
| Format document | `⇧⌥F` | `Shift+Alt+F` | Format entire document |
| Format selection | `⌘K ⌘F` | `Ctrl+K Ctrl+F` | Format selected text |

### Comments
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Toggle line comment | `⌘/` | `Ctrl+/` | Toggle line comment |
| Toggle block comment | `⇧⌥A` | `Shift+Alt+A` | Toggle block comment |
| Add line comment | `⌘K ⌘C` | `Ctrl+K Ctrl+C` | Add line comment |
| Remove line comment | `⌘K ⌘U` | `Ctrl+K Ctrl+U` | Remove line comment |

---

## 🎯 Multi-Cursor & Selection

### Multi-Cursor Operations
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Insert cursor | `⌥ + click` | `Alt + click` | Add cursor at click position |
| Insert cursor above/below | `⌥⌘↑/⌥⌘↓` | `Ctrl+Alt+↑/Ctrl+Alt+↓` | Add cursor above/below |
| Undo last cursor operation | `⌘U` | `Ctrl+U` | Undo last cursor action |
| Insert cursor at end of lines | `⇧⌥I` | `Shift+Alt+I` | Add cursor at end of each selected line |

### Text Selection
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Select current line | `⌘L` | `Ctrl+L` | Select entire line |
| Select all occurrences | `⇧⌘L` | `Ctrl+Shift+L` | Select all instances of selection |
| Select all occurrences of word | `⌘F2` | `Ctrl+F2` | Select all instances of current word |
| Add selection to next match | `⌘D` | `Ctrl+D` | Add next occurrence to selection |
| Expand/shrink selection | `⌃⇧⌘→/⌃⇧⌘←` | `Shift+Alt+→/Shift+Alt+←` | Smart expand/shrink selection |

### Column (Box) Selection
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Column selection | `⇧⌥ + drag` | `Shift+Alt + drag` | Column selection with mouse |
| Column selection up/down | `⇧⌥⌘↑/⇧⌥⌘↓` | `Ctrl+Shift+Alt+↑/Ctrl+Shift+Alt+↓` | Column selection up/down |
| Column selection left/right | `⇧⌥⌘←/⇧⌥⌘→` | `Ctrl+Shift+Alt+←/Ctrl+Shift+Alt+→` | Column selection left/right |

---

## 🔍 Search & Replace

### Basic Search
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Find | `⌘F` | `Ctrl+F` | Open find dialog |
| Find next/previous | `⌘G/⇧⌘G` | `F3/Shift+F3` | Find next/previous match |
| Replace | `⌥⌘F` | `Ctrl+H` | Open replace dialog |
| Replace in files | `⇧⌘H` | `Ctrl+Shift+H` | Find and replace across files |

### Advanced Search
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Show Search panel | `⇧⌘F` | `Ctrl+Shift+F` | Open global search |
| Select all Find matches | `⌥Enter` | `Alt+Enter` | Select all search matches |
| Move to next Find match | `⌘K ⌘D` | `Ctrl+K Ctrl+D` | Skip current and find next |

---

## 🧠 Code Intelligence

### IntelliSense & Suggestions
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Trigger suggestion | `⌃Space` | `Ctrl+Space` | Manual trigger IntelliSense |
| Trigger parameter hints | `⇧⌘Space` | `Ctrl+Shift+Space` | Show parameter hints |
| Quick Fix | `⌘.` | `Ctrl+.` | Show quick fix suggestions |

### Navigation
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Go to Definition | `F12` | `F12` | Jump to definition |
| Peek Definition | `⌥F12` | `Alt+F12` | Peek definition inline |
| Open Definition to side | `⌘K F12` | `Ctrl+K F12` | Open definition in split |
| Go to References | `⇧F12` | `Shift+F12` | Show all references |
| Rename Symbol | `F2` | `F2` | Rename symbol across files |

### Symbol Navigation
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Show all Symbols | `⌘T` | `Ctrl+T` | Search symbols across workspace |
| Go to Symbol in file | `⇧⌘O` | `Ctrl+Shift+O` | Navigate to symbol in current file |
| Go to Line | `⌃G` | `Ctrl+G` | Jump to specific line number |

---

## 📱 Panel & View Management

### Sidebar & Panels
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Toggle Sidebar | `⌘B` | `Ctrl+B` | Show/hide sidebar |
| Show Explorer | `⇧⌘E` | `Ctrl+Shift+E` | Open file explorer |
| Show Source Control | `⌃⇧G` | `Ctrl+Shift+G` | Open Git panel |
| Show Debug | `⇧⌘D` | `Ctrl+Shift+D` | Open debug panel |
| Show Extensions | `⇧⌘X` | `Ctrl+Shift+X` | Open extensions panel |
| Show Problems | `⇧⌘M` | `Ctrl+Shift+M` | Show problems panel |
| Show Output | `⇧⌘U` | `Ctrl+Shift+U` | Show output panel |

### Editor Layout
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Split editor | `⌘\` | `Ctrl+\` | Split editor vertically |
| Toggle editor layout | `⌥⌘0` | `Shift+Alt+0` | Toggle editor layout |
| Focus editor groups | `⌘1/⌘2/⌘3` | `Ctrl+1/Ctrl+2/Ctrl+3` | Focus specific editor group |
| Navigate editor groups | `⌘K ⌘←/⌘K ⌘→` | `Ctrl+K Ctrl+←/Ctrl+K Ctrl+→` | Move between editor groups |

---

## 📁 File Management

### File Operations
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| New File | `⌘N` | `Ctrl+N` | Create new file |
| Open File | `⌘O` | `Ctrl+O` | Open file dialog |
| Save | `⌘S` | `Ctrl+S` | Save current file |
| Save As | `⇧⌘S` | `Ctrl+Shift+S` | Save with new name |
| Save All | `⌥⌘S` | `Ctrl+K S` | Save all open files |
| Close editor | `⌘W` | `Ctrl+W` | Close current editor |
| Close All | `⌘K ⌘W` | `Ctrl+K Ctrl+W` | Close all editors |
| Reopen closed editor | `⇧⌘T` | `Ctrl+Shift+T` | Restore last closed file |

### File Navigation
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Copy path of active file | `⌘K P` | `Ctrl+K P` | Copy file path to clipboard |
| Reveal in Finder/Explorer | `⌘K R` | `Ctrl+K R` | Show file in system explorer |
| Open in new window | `⌘K O` | `Ctrl+K O` | Open file in new window |

---

## 🖥️ Terminal

### Terminal Operations
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Show integrated terminal | `⌃`` | `Ctrl+`` | Toggle terminal panel |
| Create new terminal | `⌃⇧`` | `Ctrl+Shift+`` | Create new terminal instance |
| Terminal command generation | `⌘K` | `Ctrl+K` | Generate terminal commands with AI |
| Run generated command | `⌘Enter` | `Ctrl+Enter` | Execute AI-generated command |
| Accept command | `Esc` | `Esc` | Accept command suggestion |

### Terminal Navigation
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Scroll up/down | `⌘↑/⌘↓` | `Ctrl+↑/Ctrl+↓` | Scroll terminal output |
| Scroll page up/down | `PgUp/PgDn` | `PgUp/PgDn` | Page through terminal |
| Scroll to top/bottom | `⌘Home/⌘End` | `Ctrl+Home/Ctrl+End` | Jump to terminal start/end |

---

## 🐛 Debug Operations

### Debug Controls
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Toggle breakpoint | `F9` | `F9` | Add/remove breakpoint |
| Start/Continue debugging | `F5` | `F5` | Start or continue execution |
| Step into | `F11` | `F11` | Step into function |
| Step out | `⇧F11` | `Shift+F11` | Step out of function |
| Step over | `F10` | `F10` | Step over line |
| Stop debugging | `⇧F5` | `Shift+F5` | Stop debug session |
| Show hover info | `⌘K ⌘I` | `Ctrl+K Ctrl+I` | Show variable info on hover |

---

## 🎨 Display & UI

### Zoom & View
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Zoom in/out | `⌘=/⇧⌘-` | `Ctrl+=/Ctrl+-` | Increase/decrease zoom |
| Toggle word wrap | `⌥Z` | `Alt+Z` | Toggle line wrapping |
| Toggle minimap | N/A | N/A | Toggle code minimap |

### Code Folding
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Fold/unfold region | `⌥⌘[/⌥⌘]` | `Ctrl+Shift+[/Ctrl+Shift+]` | Fold/unfold code block |
| Fold all subregions | `⌘K ⌘[/⌘K ⌘]` | `Ctrl+K Ctrl+[/Ctrl+K Ctrl+]` | Fold/unfold all sub-blocks |
| Fold/unfold all regions | `⌘K ⌘0/⌘K ⌘J` | `Ctrl+K Ctrl+0/Ctrl+K Ctrl+J` | Fold/unfold everything |

---

## 🚀 Advanced Cursor Features

### Composer Management
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Create new composer | `⌘N` or `⌘R` | `Ctrl+N` or `Ctrl+R` | Start new composer session |
| Close composer | `⌘W` | `Ctrl+W` | Close composer window |
| Open composer as bar | `⌘⇧K` | `Ctrl+Shift+K` | Open composer in bar mode |
| Previous/Next composer | `⌘[/⌘]` | `Ctrl+[/Ctrl+]` | Navigate composer history |

### AI History & Context
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Chat & Composer history | `⌘⌥L` | `Ctrl+Alt+L` | Open AI interaction history |
| Toggle input focus | `⌘⇧K` | `Ctrl+Shift+K` | Focus input field |
| Ask quick question | `⌥Enter` | `Alt+Enter` | Quick AI query |
| Toggle file reading strategies | `⌘M` | `Ctrl+M` | Change file context strategy |

---

## 📝 Markdown & Documentation

### Markdown Preview
| Command | Mac | Windows/Linux | Description |
|---------|-----|---------------|-------------|
| Open Markdown preview | `⇧⌘V` | `Ctrl+Shift+V` | Preview markdown file |
| Open preview to side | `⌘K V` | `Ctrl+K V` | Side-by-side markdown preview |

---

## ⚙️ Customization Tips

### Keyboard Shortcut Customization
1. Open keyboard shortcuts editor: `⌘K ⌘S` (Mac) / `Ctrl+K Ctrl+S` (Windows)
2. Search for specific commands
3. Click the pencil icon to modify shortcuts
4. Use JSON mode for advanced customization

### Recommended Practices
- **Learn Incrementally**: Master 2-3 shortcuts per week
- **Focus on Frequency**: Learn shortcuts for actions you do most often  
- **Muscle Memory**: Practice regularly to build automatic responses
- **Customize**: Adapt shortcuts to match your workflow
- **AI-First**: Leverage Cursor's unique AI shortcuts for maximum productivity

---

## 🔧 Troubleshooting

### Common Issues
- **Shortcuts not working**: Check for conflicting system shortcuts
- **AI features unresponsive**: Verify API connection and model availability
- **Custom shortcuts ignored**: Ensure proper JSON formatting in keybindings.json
- **Context not loading**: Try refreshing codebase index with `@codebase`

### Getting Help
- Use `⌘⇧P` (Mac) / `Ctrl+Shift+P` (Windows) → "Help: Show All Commands"
- Press `⌘R` then `⌘S` in Cursor to see all available shortcuts
- Check [Cursor Community Forum](https://forum.cursor.com/) for support

---

*Last updated: January 2025*  
*Sources: Cursor101, Starmorph Blog, Mehmet Baykar, Cursor Community Forum*
