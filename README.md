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

## Contributors

The main part of the extension is the `bjam.tmLanguage.json` file.
This file contains language grammar for [Boost.Jam](http://boost.org/build/) syntax highlighting.
The file was written from scratch and not converted from any existing TextMate grammar.

If you want to provide a fix or improvement, awesome!
Please improve the file and create a pull request against this git repository.

All contributions are welcome!

## License

[MIT](https://github.com/twxs/vs.language.cmake/blob/master/LICENSE)

**Enjoy!**
