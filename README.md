# Cram README

[Cram](https://pypi.python.org/pypi/cram) is a functional testing framework for command line applications. Cram tests look like snippets of interactive shell sessions. Cram runs each command and compares the command output in the test with the command’s actual output.

## Features

The extension provides a syntax definition for the Cram language.

The syntax definition is a superset of bash. Cram only has a simple markers indented at column 3 (two spaces indentation), to differentiate command lines (which start with `'$'`) to expected output lines. Like in bash, you can also have commands spread on multiple lines marking the command line with the `'>'` character instead. Comments lines bare no indentation and they can be written with ease.

For example, this is how the extension is highlighted in VS Code:

![syntax highlight example](images/syntax01.png)

> Note: The Cram language is sensitive to whitespace. Make sure to have any kind of formatting disabled in your IDE, such as tabs instead of spaces, predefined indentation, etc.

## Known Issues

Language syntax issues:
- commands declaring multi-line functions

# Release Notes

### [0.2.0] - 2019-02-18

- Fixed support for heredoc strings
- Fixed syntax highlight for comments starting with `.`

### [0.1.0] - 2016-05-01

- Basic syntax highlight for Cram language

## License

[MIT](LICENSE)

**Enjoy!**
