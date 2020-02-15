# Segmentation

[![licence](https://img.shields.io/github/license/nitely/nim-segmentation.svg?style=flat-square)](https://raw.githubusercontent.com/nitely/nim-segmentation/master/LICENSE)

An implementation of [Unicode Text Segmentation](https://unicode.org/reports/tr29/)

> See [nim-graphemes](https://github.com/nitely/nim-graphemes) for grapheme cluster segmentation

## Install

```
nimble install segmentation
```

# Compatibility

Nim +1.0.4

## Usage

```nim
import sequtils
import segmentation

assert toSeq("The (“brown”) fox can’t jump 32.3 feet, right?".words) ==
  @["The", " ", "(", "“", "brown", "”", ")", " ", "fox", " ",
    "can’t", " ", "jump", " ", "32.3", " ", "feet", ",", " ",
    "right", "?"]
```

## Docs

[Read the docs](https://nitely.github.io/nim-segmentation/)

## Tests

```
nimble test
```

## LICENSE

MIT