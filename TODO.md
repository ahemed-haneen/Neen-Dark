# Neen Dark Theme - Development Todo

## Phase 1: Foundation & Setup
- ✅ 1.1 - Create package.json with theme contribution
- ✅ 1.2 - Set up extension folder structure (themes/)
- ✅ 1.3 - Create comprehensive README documentation
- ✅ 1.4 - Initialize git repository
- ✅ 1.5 - Create QUICKSTART.md for setup guide (merged into README)
- ✅ 1.6 - Create LICENSE file

## Phase 2: Core Color Palette
- 2.1 - Define primary colors (brand colors)
- 2.2 - Define accent colors
- 2.3 - Define neutrals (whites, grays, blacks)
- 2.4 - Define semantic colors (success, warning, error, info)
- 2.5 - Test colors for contrast/accessibility

## Phase 3: Workbench UI Colors
- 3.1 - Activity Bar styling (background, icons, badges)
- 3.2 - Side Bar styling (background, borders, active/inactive)
- 3.3 - Title Bar & Menu Bar styling
- 3.4 - Status Bar styling (backgrounds, foreground, borders)
- 3.5 - Panel & Output styling
- 3.6 - Notification styling (info, warning, error)
- 3.7 - Command Palette & Quick Pick styling
- 3.8 - Tabs styling (active/inactive, icons, badges)
- 3.9 - Breadcrumb styling
- 3.10 - Welcome page styling

## Phase 4: Editor Colors
- 4.1 - Editor background & foreground
- 4.2 - Line numbers & rulers
- 4.3 - Cursor & selection colors
- 4.4 - Whitespace & indent guide colors
- 4.5 - Bracket matching & highlighting
- 4.6 - Folding & gutter colors
- 4.7 - Find & replace colors
- 4.8 - Word highlight colors
- 4.9 - Links and URL styling
- 4.10 - Error/warning squiggles & underlines
- 4.11 - Diff editor colors

## Phase 5: Syntax Highlighting (Token Colors)
- 5.1 - Comments (single-line, multi-line, doc)
- 5.2 - Strings & escape sequences
- 5.3 - Numbers & constants
- 5.4 - Keywords & control flow
- 5.5 - Variables (local, parameters, global)
- 5.6 - Functions & method names
- 5.7 - Class & type names
- 5.8 - Operators & punctuation
- 5.9 - Tags & markup (HTML/XML)
- 5.10 - Attributes & properties
- 5.11 - Invalid/error text styling
- 5.12 - Language-specific tokens (Python, JavaScript, etc.)

## Phase 6: Terminal Colors
- 6.1 - Terminal background
- 6.2 - ANSI black, red, green, yellow
- 6.3 - ANSI blue, magenta, cyan, white
- 6.4 - ANSI bright variants
- 6.5 - Terminal cursor & selection
- 6.6 - Terminal text styling

## Phase 7: Debugger & Console
- 7.1 - Debug console styling
- 7.2 - Breakpoint colors & styling
- 7.3 - Debug exception colors
- 7.4 - Call stack highlighting
- 7.5 - Variables panel styling

## Phase 8: Testing & Validation
- 8.1 - Test explorer colors
- 8.2 - Test passed/failed/skipped colors
- 8.3 - Coverage highlighting
- 8.4 - Test result styling

## Phase 9: Git & Source Control
- 9.1 - Git added file color
- 9.2 - Git modified file color
- 9.3 - Git deleted file color
- 9.4 - Git conflicted file color
- 9.5 - Diff colors (added/removed/modified)
- 9.6 - Blame styling

## Phase 10: Input & Prompts
- 10.1 - Input field styling
- 10.2 - Dropdown & select styling
- 10.3 - Focus & hover states
- 10.4 - Validation feedback colors
- 10.5 - Button styling (primary, secondary)

## Phase 11: Badges & Labels
- 11.1 - Badge background & foreground
- 11.2 - File & folder badges
- 11.3 - Error/warning badges
- 11.4 - Status badges

## Phase 12: Focus & Hover States
- 12.1 - Focus border styling
- 12.2 - Hover background colors
- 12.3 - Active state styling
- 12.4 - Disabled state styling

## Phase 13: Accessibility
- 13.1 - High contrast options for WCAG compliance
- 13.2 - Color blindness testing
- 13.3 - Focus indicator visibility
- 13.4 - Text contrast ratios
- 13.5 - Create accessibility documentation

## Phase 14: Icon Theme (Optional)
- 14.1 - Define icon design language
- 14.2 - Create file type icons
- 14.3 - Create folder icons
- 14.4 - Create status icons
- 14.5 - Create activity bar icons

## Phase 15: Documentation & Publishing
- 15.1 - Create detailed README with screenshots
- 15.2 - Create CHANGELOG
- 15.3 - Create CONTRIBUTING guidelines
- 15.4 - Create screenshot gallery
- 15.5 - Publish to VS Code Marketplace

## Phase 16: Maintenance & Community
- 16.1 - Collect user feedback
- 16.2 - Fix bug reports
- 16.3 - Support language/extension-specific requests
- 16.4 - Create theme variants (dark, light, high contrast)
- 16.5 - Keep up with VS Code updates

---

## Quick Reference

### Development Workflow
1. Edit theme file: `vscode-custom-theme/themes/custom-dark-color-theme.json`
2. Reload VS Code window: `Cmd+R` (macOS) or `Ctrl+R`
3. Test across multiple file types
4. Mark items complete as you finish

### Useful Commands
- `F5` - Start debugging/open extension in dev window
- `Cmd+Shift+P` - Open command palette
- `Cmd+Shift+P` → "color theme" - Select theme
- `Cmd+Shift+P` → "Inspect Editor Tokens and Scopes" - Debug token colors

### Color References
- VS Code Theme Docs: https://code.visualstudio.com/docs/getstarted/theme-color-reference
- Web Color Picker: https://htmlcolorcodes.com/
- Contrast Checker: https://webaim.org/resources/contrastchecker/

### Project Structure
```
Neen-Dark/
├── .git/
├── README.md             (comprehensive docs)
├── TODO.md               (this file)
├── CHANGELOG.md
├── LICENSE
├── .gitignore
└── vscode-custom-theme/
    ├── package.json
    └── themes/
        ├── custom-dark-color-theme.json
        └── custom-light-color-theme.json
```

---

## Color Palette Template (To Be Filled In)

Use this template to define your theme colors:

```
Primary Colors:
- Primary: #XXXXXX
- Secondary: #XXXXXX
- Accent: #XXXXXX

Semantic Colors:
- Success: #XXXXXX
- Warning: #XXXXXX
- Error: #XXXXXX
- Info: #XXXXXX

Neutrals:
- Black: #XXXXXX
- Dark Gray: #XXXXXX
- Gray: #XXXXXX
- Light Gray: #XXXXXX
- White: #XXXXXX
```

---

## Notes
- Prioritize workbench UI foundation before syntax highlighting
- Test accessibility at each phase
- Keep color palette consistent across light/dark variants
- Document decisions in CHANGELOG.md
- Use conventional commits for clear history
- Start with solid workbench foundation before diving into token colors
- Test with various file types (Python, JavaScript, JSON, Markdown, etc.)
- Use VS Code's built-in theme preview for real-time feedback
- Consider dark/light variants early in planning
- Keep color definitions DRY by using variables where possible
