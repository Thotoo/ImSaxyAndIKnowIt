# ImSaxyAndIKnowIt

Syntax highlighting for the SAX16 assembly language in Visual Studio Code.

## Features

- Syntax highlighting for SAX16 instructions.
- Label highlighting and declarations.
- Macro definition highlighting.
- Syntax highlighting for integer types such as `int8`, `int16`, and `int32`.
- Highlighting for pointers, constants, numbers, strings, and comments.
- Custom **SAX16 Dark** color theme.

## Supported Syntax

| Syntax | Examples |
|---|---|
| Instructions | `set16`, `add16`, `call`, `ret` |
| Labels | `start:` |
| Types | `int8`, `int16`, `int32` |
| Pointers | `*value`, `**value` |
| Constants | `true`, `false`, `null` |
| Numbers | `42`, `0xFF` |
| Strings | `'Hello, world!'` |
| Comments | `# This is a comment` |
| Macros | `macro NAME` |

The exact instructions and syntax highlighted depend on the grammar rules included in the extension.

## Installation

### Install from a VSIX file

1. Download or build the `.vsix` package.
2. Open Visual Studio Code.
3. Open the Extensions view with `Ctrl+Shift+X`.
4. Open the `...` menu.
5. Select **Install from VSIX...**.
6. Select the `.vsix` file.

### Build from source

Clone or download this repository, then run:

```bash
npm install
npm run compile
npx @vscode/vsce package
```

This creates a `.vsix` package in the project directory.

## Usage

1. Open a file with the `.sax16` extension.
2. Syntax highlighting should activate automatically.
3. To use the custom theme, open the Command Palette with `Ctrl+Shift+P`.
4. Select **Preferences: Color Theme**.
5. Choose **SAX16 Dark**.

## Development

The extension uses a TextMate grammar defined in:

```text
syntaxes/sax16.tmLanguage.json
```

The custom color theme is defined in:

```text
themes/sax16-dark-color-theme.json
```

Language configuration is stored in:

```text
language-configuration.json
```

After changing the TypeScript extension code, rebuild it with:

```bash
npm run compile
```

To test the extension during development, open the project in VS Code and press `F5` to launch an Extension Development Host.

## Contributing

Suggestions, bug reports, and improvements to the SAX16 grammar are welcome.

## License

No license has been specified yet. Add a `LICENSE` file before distributing the project if you want to make its reuse and redistribution terms explicit.
