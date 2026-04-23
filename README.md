# Lynu Language — VSCode Extension

Full language support for **Lynu** (`.lyn` files) in Visual Studio Code.

## Features

### Syntax Highlighting
Every token of the Lynu language is highlighted:

| Category | Tokens |
|---|---|
| **Declarations** | `set`, `let`, `fn` |
| **Control flow** | `if`, `then`, `else`, `end`, `loop`, `repeat`, `times`, `do`, `break`, `skip`, `give` |
| **I/O** | `say`, `print` |
| **Modules** | `use` |
| **Word operators** | `is`, `isnt`, `above`, `below`, `atleast`, `atmost`, `also`, `and`, `or`, `not` |
| **Types** | `num`, `text`, `bool`, `void` |
| **Built-ins** | `textof`, `numof`, `size`, `push`, `pop`, `input`, `type` |
| **Literals** | strings, numbers, `true`/`false` |
| **Operators** | `+`, `-`, `*`, `/`, `%`, `=`, `->`, `==`, `!=`, `>=`, `<=`, `>`, `<` |
| **Comments** | `-- line comment`, `--- block comment ---` |

### Snippets
| Prefix | Inserts |
|---|---|
| `set` | Immutable variable |
| `let` | Mutable variable |
| `fn` | Function with return type |
| `fnvoid` | Void function |
| `if` | If statement |
| `ifelse` | If/Else |
| `ifelseif` | If/Else if/Else chain |
| `loop` | Infinite loop with break |
| `repeat` | Repeat N times |
| `repeatas` | Repeat N times with index |
| `say` | Print statement |
| `use` | Use module |
| `arr` | Array literal |
| `obj` | Object literal |
| `textof` | Convert to text |
| `numof` | Convert to num |
| `input` | Read user input |
| `factorial` | Recursive factorial example |
| `hello` | Hello World |

### Themes
- **Lynu Dark** — dark background with purple/blue accent palette
- **Lynu Light** — light background with One Light-inspired palette

### Language Configuration
- Auto-closing pairs: `()`, `[]`, `{}`, `""`
- Block comment toggle: `---`
- Line comment toggle: `--`
- Auto-indent on `do`, `then`, `else`
- De-indent on `end`, `else`
- Code folding on `do`/`end` blocks

## Usage

Files ending in `.lyn` are automatically detected as Lynu. To manually set the language, use the language picker in the bottom-right of VSCode and select **Lynu**.

## Example

```lynu
-- Factorial example
fn faktorial(n: num) -> num do
    if n below 2 then
        give 1
    end
    give n * faktorial(n - 1)
end

set vysledek = faktorial(10)
say "10! = " + textof(vysledek)
```
