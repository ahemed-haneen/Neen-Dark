# Neen-Dark

A Visual Studio Code Theme Extension with vibrant colors on a dark background.

## ⚡ Quick Start (5 Minutes)

### 1. Open the Extension Folder
```bash
cd vscode-custom-theme
code .
```

### 2. Start Debugging
- Press **F5** or go to **Run > Start Debugging**
- A new VS Code window opens with your theme loaded (Development Host)

### 3. Apply the Theme
In the development window:
- Press `Cmd+Shift+P` (or `Ctrl+Shift+P`)
- Type: `color theme`
- Select "Custom Dark" or "Custom Light"

### 4. Make Your First Edit
1. In the main VS Code, edit `vscode-custom-theme/themes/custom-dark-color-theme.json`
2. Change a color, e.g., `"statusBar.background": "#FF0000"` (red)
3. In the dev window, press `Cmd+R` (or `Ctrl+R`) to reload
4. You should see the status bar turn red!

### 5. Revert & Test More
Change it back to `"#007ACC"` and reload to verify.

## 📁 Project Structure

```
Neen-Dark/
├── README.md                    # This file - all documentation
├── TODO.md                      # Development checklist (16 phases)
├── CHANGELOG.md                 # Version history
├── LICENSE                      # MIT License
├── .gitignore                   # Git ignore rules
└── vscode-custom-theme/
    ├── package.json             # Extension manifest
    └── themes/
        ├── custom-dark-color-theme.json
        └── custom-light-color-theme.json
```

## 🎨 Theme Features

- **Dark Color Theme** - Optimized for low-light environments
- **Light Color Theme** - Alternative light variant
- **Comprehensive Coverage** - 16 phases covering all UI and syntax elements
- **Accessibility Focus** - WCAG-compliant color contrasts

## 📝 Color Structure

### colors Object (Workbench & UI)

```json
"colors": {
  "focusBorder": "#007ACC",           // Focus border color
  "editor.background": "#1E1E1E",     // Editor background
  "statusBar.background": "#007ACC",  // Status bar background
  // ... 80+ more properties
}
```

### tokenColors Array (Syntax)

```json
"tokenColors": [
  {
    "name": "Comment",
    "scope": ["comment"],
    "settings": {
      "foreground": "#6A9955",
      "fontStyle": "italic"
    }
  }
  // ... more token definitions
]
```

## 🎨 Theme Architecture

The theme is organized into **16 phases**:

| Phase | Focus |
|-------|-------|
| 1 | Foundation & Setup |
| 2 | Color Palette |
| 3 | Workbench UI (Activity Bar, Sidebar, Tabs, Status Bar) |
| 4 | Editor Colors (Backgrounds, Cursors, Selections) |
| 5 | Syntax Highlighting (Comments, Strings, Keywords, Tokens) |
| 6 | Terminal (ANSI colors) |
| 7 | Debugger |
| 8 | Testing |
| 9 | Git/Source Control |
| 10 | Input & Prompts |
| 11 | Badges & Labels |
| 12 | Focus & Hover States |
| 13 | Accessibility |
| 14 | Icon Theme (Optional) |
| 15 | Documentation & Publishing |
| 16 | Maintenance & Community |

## 🎯 Development Workflow

```
1. Edit theme file in main VS Code
   └─ File: vscode-custom-theme/themes/custom-dark-color-theme.json

2. Reload development window
   └─ Press Cmd+R (macOS) or Ctrl+R (Windows/Linux)

3. See changes in real-time in dev window

4. Test different file types (.js, .py, .html, .json, .md)

5. Mark items complete in TODO.md

6. Commit changes
   └─ git commit -m "Phase 2: Add color palette"
```

## 📋 Development Checklist

Track your progress in **TODO.md**. The file organizes work into 16 phases across all aspects of the theme. Start with **Phase 2: Core Color Palette** and work through systematically.

## 🔍 Key Color Properties to Customize

### Workbench (UI Shell)
- `activityBar.*` - Left activity bar
- `sideBar.*` - File explorer sidebar
- `tab.*` - Editor tabs
- `statusBar.*` - Bottom status bar
- `titleBar.*` - Top title bar
- `editor.*` - Main editor area

### Editor
- `editor.background` / `editor.foreground` - Main colors
- `editor.lineNumber.*` - Line number styling
- `editor.cursor.*` - Cursor appearance
- `editor.selection.*` - Text selection colors
- `editorBracketMatch.*` - Bracket pairing

### Terminal
- `terminal.background` / `terminal.foreground` - Main terminal colors
- `terminal.ansi*` - ANSI color codes (16 colors)
- `terminal.ansiBright*` - Bright variants

### Syntax (Token Colors)
- `comment` - All comments
- `string` - String literals
- `keyword` - Language keywords
- `variable` - Variables
- `entity.name.function` - Function names
- `entity.name.class` - Class names
- `constant.numeric` - Numbers

## 🔧 Common Tasks

### Finding Colors to Edit

**Search by name:**
```
Press Cmd+F in VS Code, search for "statusBar"
Find all properties related to status bar
```

**Search by section:**
```
Look for comment headers like:
// ============================================
// PHASE 3: STATUS BAR
// ============================================
```

### Editing Colors

**Change a UI Color:**
```json
"statusBar.background": "#YOUR_NEW_HEX_VALUE"
```

**Add a Token Color:**
```json
{
  "name": "Your Description",
  "scope": ["scope.name"],
  "settings": {
    "foreground": "#XXXXXX",
    "fontStyle": "bold"
  }
}
```

### Testing Your Changes

1. **In Dev Window:**
   - Create test files: `test.js`, `test.py`, `test.html`
   - Type code to see syntax colors
   - Open terminal with `` Ctrl+` ``
   - Check different UI elements

2. **Use Inspector:**
   - Press Cmd+Shift+P
   - Type: `Inspect Editor Tokens and Scopes`
   - Click on text to see its scope/token
   - Match that scope to a tokenColors entry

3. **Check Contrast:**
   - Use https://webaim.org/resources/contrastchecker/
   - Aim for at least 4.5:1 ratio for normal text

### Useful Commands

| Command | Mac | Windows/Linux | Purpose |
|---------|-----|---------------|---------|
| Start Debug | F5 | F5 | Open dev window |
| Reload Window | Cmd+R | Ctrl+R | Reload theme in dev |
| Color Theme | Cmd+Shift+P → theme | Ctrl+Shift+P → theme | Switch active theme |
| Find Text | Cmd+F | Ctrl+F | Search in file |
| Replace | Cmd+H | Ctrl+H | Find & replace |
| Inspect Tokens | Cmd+Shift+P → inspect | Ctrl+Shift+P → inspect | Debug token colors |

## 🧪 Testing Your Theme

### Test with Different File Types

Create sample files to test syntax highlighting:

```bash
# Create test files in the extension folder
cd vscode-custom-theme
touch test.py test.js test.html test.json test.md
```

Open each file type and verify syntax colors look right.

### Tools for Color Picking

- **Color Picker**: VS Code has built-in color pickers (click on hex values)
- **Online Tools**: https://www.color-hex.com/
- **Contrast Checker**: https://webaim.org/resources/contrastchecker/

### Test Specific Elements

| Element | How to Test |
|---------|------------|
| Activity Bar | Look at left sidebar icons |
| Status Bar | Look at bottom status bar |
| Syntax Colors | Open Python/JS/HTML files |
| Brackets | Type matching brackets |
| Find Box | Press Cmd+F |
| Terminal | Open integrated terminal |
| Notifications | Run command, trigger error |

## 💡 Best Practices

### Color Selection
- **Contrast**: Ensure text is readable (WCAG AA = 4.5:1 ratio)
- **Consistency**: Use a limited palette (8-12 main colors)
- **Harmony**: Choose colors that work well together
- **Brand**: Reflect your personal or company style

### File Organization
- Keep `colors` and `tokenColors` organized by section
- Use comments to separate phases
- Define colors consistently (use 6-digit hex codes)
- Group related properties

### Performance
- Avoid too many custom token scopes
- Keep file size reasonable (< 50KB)
- Test accessibility at each phase
- Support colorblind-friendly modes

## 📚 External Resources

- [VS Code Theme Colors Reference](https://code.visualstudio.com/docs/getstarted/theme-color-reference)
- [VS Code Syntax Highlighting Guide](https://code.visualstudio.com/docs/extensions/theming)
- [VS Code Extension API](https://code.visualstudio.com/api)
- [Publishing to Marketplace](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)

## 📤 Publishing

When ready to share:

1. **Update vscode-custom-theme/package.json**
   - Add author, repository, license
   - Increment version number

2. **Update CHANGELOG.md**
   - Document version history
   - Note changes and improvements

3. **Add Screenshots**
   - Create demo images showing the theme
   - Update this README

4. **Install VS Code Extension CLI**
   ```bash
   npm install -g @vscode/vsce
   ```

5. **Create Publisher Account**
   - Go to https://marketplace.visualstudio.com
   - Sign up as publisher

6. **Publish**
   ```bash
   cd vscode-custom-theme
   vsce publish
   ```

## 🤝 Contributing

Have ideas? Follow this workflow:

1. Create a branch: `git checkout -b feature/amazing-colors`
2. Make changes and test thoroughly
3. Commit with clear messages
4. Push and create a pull request

## ❓ Troubleshooting

### Theme not appearing
- Reload VS Code: `Cmd+R` (macOS) or `Ctrl+R`
- Check `vscode-custom-theme/package.json` theme registration
- Verify JSON syntax (no trailing commas)

### Colors look wrong
- Inspect tokens: `Inspect Editor Tokens and Scopes` command
- Check color hex values (use online converter if unsure)
- Test contrast ratio for readability
- Verify scope names match file syntax

### JSON errors
- Use VS Code's built-in JSON validator
- Check for trailing commas
- Ensure all quotes are proper (`"not '`)
- Use an online JSON validator

## 📄 License

MIT - See [LICENSE](LICENSE) file for details.

## 👤 Author

Your Name (customize in vscode-custom-theme/package.json)

---

## Next Steps

1. **Run the quick start above** - Get the dev environment running (5 minutes)
2. **Open TODO.md** - See all phases and development items
3. **Start with Phase 2** - Pick your color palette (10-15 minutes)
4. **Edit vscode-custom-theme/themes/custom-dark-color-theme.json** - Add your colors
5. **Test in dev window** - Reload (Cmd+R) and verify
6. **Work through phases** - Move systematically through TODO.md

Happy theming! 🎨
