## Color

This specimen is configured with a JSON array as the content. 

Name is optional.

### Keys

- __`value: string`__ defines the color
- `name: string` defines the color name

### Options

- `span-[1-6]` defines the width of the palette


### Examples

#### Color swatch

The color swatches are useful to document single or important colors like the main brand scheme.

```color|span-3
{"name": "Light Blue", "value": "#b0f6ff"}
```

```color|span-2
{"name": "Dark Blue",  "value": "#2666a4"}
```

```color|span-1
{"name": "Bright Red",  "value": "#ff5555"}
```

```code|lang-javascript
'''color|span-3
{"name": "Light Blue", "value": "#b0f6ff"}
'''

'''color|span-2
{"name": "Dark Blue",  "value": "#2666a4"}
'''

'''color|span-1
{"name": "Bright Red",  "value": "#ff5555"}
'''
```


### Color palette

Catalog also has a [Color Palette Specimen](#/color-palette).
