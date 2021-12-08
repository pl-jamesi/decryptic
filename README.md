# decryptic README

Naive syntax highlighting for Decryptic (\*.dcr) files for the Delphic LIS.

## Features

Primitive support based on existing Pathlab Decryptic protocols:

<img src="https://github.com/pl-jamesi/decryptic/blob/master/images/decryptic-highlighting-example.png?raw=true" alt="Example Decryptic Highlighting" width="600px" />

## Installation

- In `<user home>/.vscode/extensions` folder `git clone https://github.com/pl-jamesi/decryptic.git` and restart VS Code.

## Known Issues

Uses inappropriate names rather than custom theming to make colouration work.

## Contributing

All the magic happens in `syntaxes/decryptic.tmLanguage.json` the Text mate grammar file that is used for tokenization.

You may find the following resources useful:

https://www.youtube.com/watch?v=5msZv-nKebI - walkthrough of someone else going through the experience of setting up syntax highlighting for their own language.

https://regexr.com/ - for testing regular expressions. Note, in .tmLanguage.json you have to double escape using \\, but regexr should only have one \ to escape something.

https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide - written instructions on set up and behaviour of VS Code syntax highlighting.

https://github.com/microsoft/vscode/blob/main/extensions/theme-defaults/themes/light_vs.json - for examples of "names" to use for colouring.

## Development

- Make changes to `syntaxes/decryptic.tmLanguage.json`
- Press `F5` to open a new window with the extension loaded.
- Create a new file with a file name suffix matching your language or otherwise manage file type association in .vscode/settings.json.
- Verify that syntax highlighting works.
- You can also reload (`Ctrl+R` or `Cmd+R` on Mac) the VS Code window with your extension to load saved changes.

## Add more language features

- There's documentation on intellisense, hovers, and validators, etc at VS Code extenders documentation at https://code.visualstudio.com/docs
- I've not implemented any of it at this time but it may be worthwhile.
