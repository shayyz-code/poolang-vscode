# Poo Language Support for Visual Studio Code

This extension adds syntax highlighting and basic support for the **Poo programming language** in Visual Studio Code. Poo is a simple, lightweight language with features like custom keywords, vector manipulations, and functional programming constructs.

## Features

- **Syntax Highlighting**:
  - Keywords: `poo`, `poof`, `mut`, `return`, `for`, `in`, `if`, `else`, `elif`
  - Standard library: `std`, `math`
  - Boolean literals: `true`, `false`
  - Numbers, strings, comments
- **File Association**: Automatically activates for `.poo` files.

## Example Code

```poo
use std::pout;

poo my_vec = ["world", "hello"];
poo a = 5.0 * 1.0 - 1.0 * 3.0;
poo b = 2 / 2;
poo mut d = true;
d = false;

poof getHelloWorld(e: vec) >> vec {
    return e;
}

for item in my_vec {
    pout("Hello, Poo!", item);
}

pout(my_vec.pop());
```

## Installation

1. Clone or download this repository.
2. Open Visual Studio Code and go to the Extensions view (`Ctrl+Shift+X` or `Cmd+Shift+X` on macOS).
3. Click the `...` menu at the top-right corner and select `Install from VSIX...`.
4. Select the `.vsix` file generated from this repository (if available) or open the folder in VS Code and run `npm install && npm run package` using the [vsce](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) CLI tool.

## Language Features

### Keywords

The following are recognized as Poo language keywords:

- `poo`: Declares variables.
- `poof`: Declares functions.
- `mut`: Marks variables as mutable.
- `return`: Returns values from functions.
- `for`, `in`: Used for iteration.

### Standard Library Functions

- **`pout`**: Outputs values to the console. Part of the standard library.

### Built-in Methods

- **`pop`**: Removes and returns the last element of a vector.

## Contributions

Contributions are welcome! Feel free to open issues, suggest features, or submit pull requests to enhance the Poo language support.

## License

This project is licensed under the MIT License.
