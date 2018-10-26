# vscode-boost-jam README

This extension provides support for [Boost.Jam](http://boost.org/build/)
language in Visual Studio Code.

Boost.Jam is an interpreted language implemented by [Boost.Build](http://boost.org/build/)
engine, `b2`, which loads the Jam code that implements the build system.

Boost.Build is developed as part of [Boost](https://boost.org) project.

## Features

- Syntax highlighting
- Code comments

## Acknowledgements

- [Matt Neuburg](https://github.com/mattneub) for his [Writing a TextMate Grammar: Some Lessons Learned](http://www.apeth.com/nonblog/stories/textmatebundle.html)
- [Michael Lovitt](http://www.lovitt.net) for [Rubular](http://www.rubular.com/)
- [Rene Rivera]() for converting Boost.Build docs to AsciiDoc
- Boost.Build developers for the excellent build system.


## Contributors

The main part of the extension is the `bjam.tmLanguage.json` file.
This file contains language grammar for [Boost.Jam](http://boost.org/build/) syntax highlighting.
The file was written from scratch and not converted from any existing TextMate grammar.

If you want to provide a fix or improvement, awesome!
Please improve the file adh create a pull request against this git repository.

## License

[MIT](https://github.com/twxs/vs.language.cmake/blob/master/LICENSE)

**Enjoy!**
