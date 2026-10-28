# ImSaxyAndIKnowIt

**Syntax highlighting for SAX16 assembly language in Visual Studio Code.**

ImSaxyAndIKnowIt adds syntax highlighting and a custom dark color theme for SAX16 assembly source files.

## Features

- Syntax highlighting for `.sax16` files
- Custom **SAX16 Dark** color theme
- Highlighting for labels and instructions
- Distinct colors for data types, pointers, numbers, strings, and comments
- Designed to make SAX16 code easier to read and navigate

## Example

The extension highlights common SAX16 language elements, including:

- **Labels** — control-flow targets and named locations
- **Instructions** — assembly operations
- **Control keywords** — directives and macro-related keywords
- **Data types** — type declarations
- **Pointers** — pointer-related syntax
- **Numbers and strings** — constants and literal values
- **Comments** — comments beginning with `#`

## Installation

### Install from a VSIX file

1. Download the latest `.vsix` file from the [GitHub Releases page](https://github.com/Thotoo/ImSaxyAndIKnowIt/releases).
2. Open Visual Studio Code.
3. Open the **Extensions** view.
4. Open the `...` menu and select **Install from VSIX...**.
5. Select the downloaded `.vsix` file.

### Select the color theme

1. Open the Command Palette with `Ctrl+Shift+P` (`Cmd+Shift+P` on macOS).
2. Search for **Preferences: Color Theme**.
3. Select **SAX16 Dark**.

## Usage

Open any file with the `.sax16` extension. The language grammar should be detected automatically, and syntax highlighting will be applied.

For the intended colors, select the **SAX16 Dark** theme.

## Development

Clone the repository:

```bash
git clone https://github.com/Thotoo/ImSaxyAndIKnowIt.git
cd ImSaxyAndIKnowIt
```

Install dependencies and compile:

```bash
npm install
npm run compile
```

Package the extension into a VSIX file:

```bash
npx @vscode/vsce package
```

The generated `.vsix` file can be installed locally in Visual Studio Code using **Install from VSIX...**.

## Known limitations

- The extension currently provides syntax highlighting and a color theme; it does not provide a SAX16 compiler, debugger, or language server.
- Syntax highlighting depends on the language grammar and the selected color theme.
