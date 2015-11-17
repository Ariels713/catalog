## Download

### Keys
- __`url: string`__ The URL pointing to the file
- __`title: string`__ The title for the button
- `filename: string` Changes the file name under which it will be saved
- `subtitle: string` For example the file size

### Arguments
- `span-[1-6]` defines the download specimen width

### Examples

#### Basic example

```download
{
    "title": "Catalog Logo (.svg)",
    "url": "docs/assets/catalog_logo.svg"
}
```

```code
'''download
{
    "title": "Catalog Logo (.svg)",
    "url": "docs/assets/catalog_logo.svg"
}
'''
```

#### Different widths

```download|span-6
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
```
```download|span-3
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
```
```download|span-3
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
```
```download|span-2
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
```
```download|span-2
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
```
```download|span-2
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
```


```code|collapsed
'''download|span-6
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
'''
'''download|span-3
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
'''
'''download|span-3
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
'''
'''download|span-2
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
'''
'''download|span-2
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
'''
'''download|span-2
{
    "title": "Catalog Logo (.svg)",
    "filename": "catalog-logo",
    "subtitle": "8 KB",
    "url": "docs/assets/catalog_logo.svg"
}
'''
```


```hint
If you want to have multiple files available for download automatically, keep in mind that the Project specimen can pack them into a .zip.
```
