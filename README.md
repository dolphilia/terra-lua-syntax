# Terra-Lua-Syntax

This extension provides enhanced syntax highlighting for Terra, a low-level system programming language that is closely integrated with Lua. It aims to support not only basic Terra syntax, but also language constructs that blend Terra and Lua, enabling a smooth development experience when working with hybrid Terra/Lua codebases.

## Features

- **Terra Keywords & Types**: Highlights all Terra-specific keywords and types (e.g., `terra`, `struct`, `int32`, `float`, etc.).
- **Lua Integration**: Includes embedded Lua syntax highlighting, ensuring that Lua code within Terra files also benefits from full syntax support.
- **Quoted Expressions**: Special handling for Terra’s quoted expressions using backticks (e.g., `` `a ``, `` `[ something ] ``), providing a clearer distinction in your code.
- **Inline C Integration**: Supports inline C code blocks introduced by `terralib.includecstring`, applying C syntax highlighting to the embedded code.
- **ASDL Grammar Blocks**: Provides syntax highlighting within `:Define[[ ... ]]` blocks for ASDL grammar definitions, highlighting keywords (`module`, `attributes`, `unique`) and tokens (`=`, `|`, `?`, `*`, `{`, `}`, etc.).

### Screenshots

*Coming soon...*

## Requirements

- **VS Code** (latest stable recommended)
- **Lua syntax support** (either built-in or via a Lua extension) for best results when embedding Lua code.
- No other special dependencies are required.

## Extension Settings

This extension currently does not add any custom VS Code settings.  
All highlighting behavior is controlled by the extension’s grammar definitions and your current theme.

## Known Issues

- State-dependent highlighting (e.g., dynamically recognized variable names after `asdl.NewContext()`) is not possible due to the limitations of TextMate grammars.
- Certain complex Terra/Lua blends may not be highlighted perfectly, but most common patterns are supported.

## Release Notes

### 1.0.0

- Initial release:  
  - Terra keywords, numbers, types, and strings highlighted.
  - Basic Lua syntax highlighting embedded.
  - Quoted expressions and inline C code blocks recognized.
  - ASDL grammar blocks (`:Define[[ ... ]]`) highlighted.

## For more information

- [Terra Language](http://terralang.org/)
- [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
- [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy using Terra with improved syntax highlighting!**
