# vscode-boost-jam

This extension provides support for [Boost.Jam](http://boost.org/build/)
language in Visual Studio Code.

![screenshot](images/screenshot.png)

Boost.Jam is an interpreted language implemented by [Boost.Build](http://boost.org/build/)
engine, `b2`, which loads the Jam code that implements the build system.
Boost.Build is developed as part of [Boost](https://boost.org) project.

## Features

- Syntax highlighting
- Code comments

Although the process of writing a TextMate language grammar remains
*poorly documented*, this is a *brave* first attempt to provide
a minimal usable support for Boost.Jam. By no means, it is free from
bugs or covers all elements of Boost.Jam language. Non-trivial TextMate
grammars for Visual Studio Code count from 500 to 5000 lines of code,
and this one *less than 200*.

## Installation

- Visual Studio Code > Extensions (CTRL+SHIFT+X)
- https://marketplace.visualstudio.com/items?itemName=mloskot.vscode-boost-jam

## Acknowledgements

- [Matt Neuburg](https://github.com/mattneub) for his [Writing a TextMate Grammar: Some Lessons Learned](http://www.apeth.com/nonblog/stories/textmatebundle.html).
- [Michael Lovitt](http://www.lovitt.net) for [Rubular](http://www.rubular.com/).
- [Rene Rivera](https://github.com/grafikrobot/) for converting Boost.Build docs to AsciiDoc.
- [Boost.Build developers](https://github.com/boostorg/build) for the excellent build system.

## Development

The main part of the extension is the `bjam.tmLanguage.json` file.
This file contains language grammar for [Boost.Jam](http://boost.org/build/) syntax highlighting.
The file was written from scratch and not converted from any existing TextMate grammar.

**If you want to offer a fix or improvement, awesome!**

Please improve the file and create a pull request against this git repository.

All contributions are welcome!

### Testing

There are no automated tests provided.
There is just `test/colorize-fixtures/test.jam` file provided,
but without company of `test/colorize-results/test_jam.json` file.
In fact, I have no idea how such tests should be implemented.

Instead, install or run the extension and open `test/colorize-fixtures/test.jam` file.
Look what you see and compare it with what you would prefer to see.
Then, hopefully, happy hacking in attempt to correct the language grammar :-)

[Running and debugging your extension](https://code.visualstudio.com/docs/extensions/developing-extensions)
explains in details how to run the extension for convenient development and testing. In short:

1. Open `vscode-boost-jam` folder in VSCode and hit F5 to start debugging.
2. New (preview) window appears with the extension loaded, in it, open the `test.jam` or your own Jamfile.
3. Edit the grammar file in the parent window.
4. Reload the debugging (preview) window with CTRL+R
5. Observe result, modify the `test.jam`.
6. Iterate over steps from 3 to 5

### Publishing

(*by original author*)

Follow the official guide on
[Publishing Extension(https://code.visualstudio.com/api/working-with-extensions/publishing-extension)
to VS Code Extension Marketplace.

## License

[MIT](https://github.com/twxs/vs.language.cmake/blob/master/LICENSE)

**Enjoy!**
