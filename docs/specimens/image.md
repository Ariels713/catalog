## Image

Images can be used as graphical elements, to document implemtation details with static images or behavioral aspects when animated gifs are used. The src and overlay keys accept the `srcSet` notation, which allows the usage of responsive images.

### Keys
- `src: string` image to display (gets scaled if it extends the container) 
- `overlay: string` image for mouseover, useful to describe proportions
- `title: string` the title 
- `description: string` Markdown-formatted text description

#### Visual
* `light` a light checkered background (default)
* `dark` a dark checkered background
* `plain` a transparent background without any padding.
* `plain,dark` a solid, dark background without the checkered pattern
* `plain,light` a solid, light background without the checkered pattern
* `span-[1-6]` defines the width


### Example: Hero Image

By using a plain background and no title you can place a simple image.

```image|plain
{
    "src": "docs/assets/image_bw.jpg"
}
```

_Example image by [unsplash](https://unsplash.com/photos/-YMhg0KYgVc)._

```code|lang-javascript
'''image|plain
{
    "src": "docs/assets/image_bw.jpg"
}
'''
```


### Example: Overlay image

The overlay image is useful to document layout measurements for implementation.

```image
{   
    "src": "docs/assets/catalog_logo.png",
    "overlay": "docs/assets/catalog_logo-overlay.png"
}
```

```code|lang-javascript
'''image
{   
    "src": "docs/assets/catalog_logo.png",
    "overlay": "docs/assets/catalog_logo-overlay.png"
}
'''
```



### Example: Image with details

By adding attributes it is possible to specify implementation details.

```image|dark
{
    "src": "docs/assets/catalog_logo.png",
    "description": "alt text: catalog logo, add .2s fade in animation",
    "title": "Catalog Logo"
}
```

```code|lang-javascript
'''image|dark
{
    "src": "docs/assets/catalog_logo.png",
    "description": "alt text: catalog logo, add .2s fade in animation",
    "title": "Catalog Logo"
}
'''
```

### Multiple images

```image|span-5
{
    "src": "docs/assets/catalog_logo.png",
}
```

```image|span-1
{
    "src": "docs/assets/catalog_logo.png",
}
```

```code|lang-javascript
'''image|span-5
{
    "src": "docs/assets/catalog_logo.png",
}
'''

'''image|span-1
{
    "src": "docs/assets/catalog_logo.png",
}
'''
```
