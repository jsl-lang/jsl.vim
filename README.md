# jsl.vim

Syntax and indent files for [JSL](https://github.com/jsl-lang)

## Installation

Use your favorite (neo)vim plugin manager or (neo)vim itself (after vim 8.0).

E.g. with Pathogen (vim):
```bash
cd ~/.vim/bundle && git clone https://github.com/jsl-lang/jsl.vim
```

Or Lazy (neovim):
```lua
return {
    "jsl.vim"
}
```

## Usage

Contains syntax, indent and filetype files for JSL.

Supports [all features of JSL](https://github.com/jsl-lang/jsl/blob/master/SCHEMA-SPEC.md) with minor exception:
```c
// This will get highlighted correctly
// Please prefer this syntax for splitting lines
node argument \
    argument

// Argument on new line will be
// highlighted as node
// Please avoid this syntax
node argument \
argument
```

Additional (fancy) features:
- Error highlight for invalid syntax
- Full escape sequence highlight
- Proper highlight for escaping newline in strings
- Full `/-` comment highlight
- Different highlight groups for each component type (including operators)

## License
MIT

