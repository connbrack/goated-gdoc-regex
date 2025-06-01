# Goated Gdoc Regex

## Quotes

### Double quotes

```
(?<=^|[ \t])"(?=\S)
(?<=\S)"(?=[ \t\n])
```

> replace with: `“ or ”`

### Single quotes

```
(?<=[" \t]|^)'(?=\S)
(?<=[^\s])'
```

> replace with `‘ or ’`

### Edge cases 

Space or non-space on both sides.

```
(?<=[ \t]|^)"(?=[ \t\n])
(?<=[ \t]|^)'(?=[ \t\n])
(?<=\S)"(?=\S)
```

> fix manually
