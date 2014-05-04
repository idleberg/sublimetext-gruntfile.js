# sublimetext-gruntfile.js

**This project is work-in-progress, [help](#contributions) is greatly appreciated!**

A simple `Gruntfile` for Sublime Text package developers to validate XML and lint JSON files.

Supported file types:

File extension         | Type | Function
-----------------------|------|---------
`.JSON-tmLanguage`     | JSON | [Sublime Text Syntax Definitions](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/syntaxdefs.html)
`.plist`               | XML  | [Property List](https://developer.apple.com/library/Mac/documentation/Darwin/Reference/ManPages/man5/plist.5.html)
`.sublime-build`       | JSON | [Sublime Text Build Systems](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/build_systems.html)
`.sublime-commands`    | JSON | [Sublime Text Command Palette](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/command_palette.html)
`.sublime-completions` | JSON | [Sublime Text Completions](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/completions.html)
`.sublime-keymap`      | JSON | [Sublime Text Key Bindings](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/key_bindings.html)
`.sublime-macro`       | JSON | [Sublime Text Macros](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/extensibility/macros.html?highlight=macro)
`.sublime-menu`        | JSON | [Sublime Text Menus](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/customization/menus.html?highlight=menu)
`.sublime-settings`    | JSON | [Sublime Text Settings](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/settings.html)
`.sublime-snippet`     | XML  | [Sublime Text Snippets](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/snippets.html)
`.sublime-theme`       | JSON | Sublime Text Theme
`.tmCommand`           | XML  | [TextMate Commands](http://manual.macromates.com/en/commands)
`.tmLanguage`          | XML  | [TextMate Language Grammars](http://manual.macromates.com/en/language_grammars)
`.tmPreferences`       | XML  | [TextMate Preferences](http://manual.macromates.com/en/preferences_items)
`.tmSnippet`           | XML  | [TextMate Snippets](http://manual.macromates.com/en/snippets)
`messages.json`        | JSON | [Package Messaging](https://sublime.wbond.net/docs/messaging)

## Usage

### Prerequisites

Download the files using [git clone](http://git-scm.com/docs/git-clone) or the [`.zip`](https://github.com/idleberg/sublimetext-gruntfile.js/archive/master.zip) file option. Place the `Gruntfile.js` and `package.json` in the folder of your Sublime Text package (or whatever files you would like to test). Unless there is a `.gitignore` file in the same folder, you should copy it as well – or add `node_modules/` to an existing file.

You also need to have npm (“Node package manager”) [installed](http://www.joyent.com/blog/installing-node-and-npm/) before you can make use of any of this.
 
### Basic Usage

1. Upon first use, perform `npm install` to download all required packages
2. Run `grunt` to run the default tests

### Optional Usage

* Use `grunt json` to lint all JSON files
* Use `grunt xml` to validate all XML files
* Use `grunt watch` to run all tasks in background while editing your files

## Contributions

I guess it would be more convenient to turn this into a Sublime Text (or npm) package, but I don't have enough experience yet to get there. Hence, I appreciate all help making this more useful for package developers.

## License

The MIT License (MIT)

Copyright (c) 2014 Jan T. Sott

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Donate

You are welcome support this project using [Flattr](https://flattr.com/submit/auto?user_id=idleberg&url=https://github.com/idleberg/sublimetext-gruntfile.js) or Bitcoin `17CXJuPsmhuTzFV2k4RKYwpEHVjskJktRd`