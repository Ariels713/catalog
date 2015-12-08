## Hint

Can be used to highlight important aspects.

### Arguments

- `directive` good for _dos_
- `warning` good for _don'ts_
- `neutral` a neutral style

### Examples

```hint
Make sure to use `text-rendering: optimizeLegibility;` on fonts over 36px, as well as `-webkit-font-smoothing: antialiased;` and `-moz-osx-font-smoothing: grayscale;` on dark backgrounds.
```

```code
'''hint
Make sure to use `text-rendering: optimizeLegibility;`on fonts over 36px, as well as `-webkit-font-smoothing: antialiased;` and `-moz-osx-font-smoothing: grayscale;` on dark backgrounds.
'''
```

```hint|directive,span-4
Make it so!
```

```code|span-2
'''hint|directive
Make it so!
'''
```

```hint|warning,span-4
No **stairway**.
```

```code|span-2
'''hint|warning
No **stairway**.
'''
```

```hint|neutral,span-4
A neutral hint.
```

```code|span-2
'''hint|neutral
A neutral hint.
'''
```

```hint|span-4
# Supports

even Markdown with [links](http://example.com)

- and
  - lists
```

```code|span-2
'''hint
# Supports

even Markdown with [links](http://example.com)

- and
  - lists
'''
```
