[SMuFL](http://smufl.org/) is a new proposed standard for music fonts, formed alongside Steinberg's in-development notation software. The first and currently the only SMuFL font is Bravura, a bold and easy-to-read typeface developed for Steinberg's program by Daniel Spreadbury. It is freely available under the SIL Open Font License.

[LilyPond](http://lilypond.org/) is a free and open-source music engraving program. This is a LilyPond script providing partial support for Bravura and other future SMuFL fonts.

## Usage ##

**Current version:** SMuFL 0.7

Make sure Bravura is installed on your system (get it from [the SMuFL website](http://www.smufl.org/fonts/)), and that `smufldata.ily` and `bravura.ily` are in the same directory. Include `\bravuraOn` (or `\smuflOn` to avoid Bravura-specific overrides) in the Staff context:

```lilypond
\new Staff {
  \bravuraOn
  c'4 d' e' c'
}
```

Or, better:

```lilypond
\score {
  % ...
  \context {
    \Staff {
      \bravuraOn
    }
  }
}
```
