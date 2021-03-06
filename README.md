_N.B. This is a fork of the_ [Source Code Pro repository](https://github.com/adobe/source-code-pro)

## Hasklig - Ligatures for Haskell code

Programming languages are limited to relatively few characters. As a result of a limited character set, combined character operators surfaced quite early, such as the widely used arrow (`->`), comprised of a hyphen and greater sign. It looks like an arrow if you know the analogy and squint a bit.

Composite glyphs are problematic in languages such as Haskell which utilize these complicated operators (`<-`, `::`, `=>`, `-<`, `>>=` etc.) extensively (_over 100 in_ `lens` _alone_!). The readability of this kind of complex code improves considerably with some kind of pretty printing.

Some Haskell programmers have resorted to unicode symbols in code as a solution (`⇒`, `←` _etc._). This opens a whole new can of worms. In addition to encoding/compatibility problems and all the reasons it never worked out for APL, these symbols are one-character-wide and therefore eye-strainingly small.

Hasklig solves this problem the way typographers have always solved ill-fitting characters which co-occur often: ligatures. The underlying code stays the same — only the representation changes.

[**Download Font Family**](https://github.com/i-tu/Hasklig/releases/download/v0.2/Hasklig_0.2.zip)

#### Hasklig
![Hasklig Sample](hasklig_example.png?raw=true)

#### Source Code Pro
![Source Code Pro Sample](SourceCodeProSample.png?raw=true)

### Editors and Terminals with support
+ Atom (_add_ `text-rendering: optimizeLegibility;` _to your_ `.editor` _css._)
+ Chocolat
+ gEdit
+ Kate
+ Konsole
+ KWrite
+ Leksah
+ TextEdit

### No support
- Aquamacs
- gVim (_output corrupted_)
- iTerm2
- MacVim
- Sublime Text (_Vote for the enhancement_ [**here**](http://sublimetext.userecho.com/topic/433445-/))
- Terminal (OSX)

## To Do
1. Contextual glyph substitution for `\` → `λ` and `.` → `∘`
2. Terminal support (for example iTerm2)
3. Discretionary or alternate ligatures for some characters (_notably_ `/=` _with a slash in the middle, and pretty printed less-equals and greater-equals signs_)
4. Version for C-esque languages (`->`, `!=`, `==`)
