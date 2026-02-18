# Minimalitch - VS Code Settings Extension

A minimalist and highly optimized VS Code configuration extension designed for a clean, distraction-free coding environment. This extension provides carefully curated default settings that enhance productivity while maintaining visual simplicity and focus.

## Overview

Minimalitch is a comprehensive configuration package for Visual Studio Code that combines aesthetic minimalism with functional optimization. It provides sensible defaults across editor rendering, workbench layout, file management, terminal appearance, and language-specific formatting rules.

The extension focuses on:

- **Clean Editor Experience**: Reduced visual clutter with hidden line numbers, minimap, and status bar
- **Minimalist UI**: Hidden activity bar, compact workbench layout, and simplified navigation
- **Optimized Rendering**: Disabled unnecessary visual decorations (bracket pairs, color decorators, code lens)
- **Smart File Management**: Intelligent exclusion patterns for cleaner file explorer navigation
- **Consistent Typography**: JetBrains Mono and MonoLisa fonts with modern ligature support across all UI elements
- **Language-Specific Formatters**: Dedicated formatting rules for PHP, Vue, Blade, JavaScript, TypeScript, and HTML
- **Terminal Integration**: Optimized terminal appearance matching the editor theme
- **Git Integration**: Minimal git decorations with optimized diff viewing

## Key Configuration Highlights

The extension modifies these core areas:

- Editor appearance (line numbers off, minimap disabled, no color decorators)
- Workbench UI (activity bar hidden, sidebar positioning, tab management)
- Rendering behavior (cursor blinking, bracket matching disabled, reduced highlights)
- Color scheme (dark background with minimal ruler colors)
- File exclusions (comprehensive patterns for cleaner navigation)
- Auto-save and formatting (Prettier integration on paste/save)
- Terminal styling (block cursor, smooth scrolling, Emmet support)
- Language formatters (PHP, Vue, Blade, JavaScript/TypeScript)
- Vim mode support (if vim extension installed)

## Extension Settings

This extension contributes the following configuration defaults:

```json
{
	"editor.guides.indentation": false,
	"editor.cursorBlinking": "blink",
	"vim.cursorStylePerMode.insert": "block",
	"scm.diffDecorations": "none",
	"editor.colorDecorators": true,
	"editor.occurrencesHighlight": "off",
	"editor.renderLineHighlight": "none",
	"editor.matchBrackets": "never",
	"editor.lightbulb.enabled": "off",
	"editor.scrollbar.vertical": "hidden",
	"editor.fontLigatures": true,
	"editor.rulers": [
		{
			"column": 0,
			"color": "#202a36"
		}
	],
	"files.exclude": {
		"**/.git": true,
		"**/.github": true,
		"**/.svn": true,
		"**/.hg": true,
		"**/.DS_Store": true,
		"**/Thumbs.db": true,
		"**/node_modules": true,
		// "**/storage": true,
		"**/bootstrap/cache": true,
		// "**/.env": true,
		"**/.env.*": true,
		"**/tests": true,
		"**/.editorconfig": true,
		"**/artisan": true,
		// "**/composer.json": true,
		"**/composer.lock": true,
		"**/phpunit.xml": true,
		"**/.eslintrc.json": true,
		"**/.gitignore": true,
		"**/.gitattributes": true,
		"**/.vscode": true,
		"**/.prettierrc": true,
		// "**/vite.config.*": true,
		"**/jsconfig.json": true,
		"**/tsconfig.json": true,
		"**/next.config.*": true,
		"**/next-env.d.ts": true,
		"**/tailwind.config.js": true,
		// "**/package.json": true,
		"**/package-lock.json": true,
		"**/yarn.lock": true,
		"**/pnpm-lock.yaml": true,
		"**/bun.lockb": true,
		"**/eslint.config.*": true,
		"**/postcss.config.*": true,
		// "**/README.md": true,
		"**/dist": true,
		"**/build": true,
		"**/.idea": true,
		"**/.next": true
	}
}
```

## Complete Configuration

For the full, detailed configuration including all editor preferences, terminal settings, language-specific formatters, keyboard bindings, color customizations, and advanced extension settings, refer to:

- **Full Settings**: [settings.json](https://github.com/phantriviethoang/vscode/blob/main/settings.json)
- **Keyboard Bindings**: [keybindings.json](https://github.com/phantriviethoang/vscode/blob/main/keybindings.json)
