## HyperText Markup Language
### Introduction to HTML
#### Element  
- The body : `<body></body>`
- Heading : `<h1-6></h1-6>`
- Div : `<div></div>`
- Plain text : `<p></p>`
- Separate pieces of content : `<span></span>`
- *Italic* emphasis : `<em></em>`
- **bold** emphasis : `<strong></strong>`
- Line Breaks : `<br>`
- Unordered Lists : `<ul></ul>`
- Ordered Lists : `<ol></ol>`
- List items : `<li></li>`
- Images : `<img src="image-location.jpg" />`
- [Image Alts] : `<img src="#" alt="A field of yellow sunflowers" />`
- Videos : 
``` html
<!-- define the width & height -->
<!-- displayed if the browser is unable to load your video -->
<video src="myVideo.mp4" width="320" height="240" controls>
    Video not supported
</video>
```

#### Attributes
- id tag : `<div id="intro">`


### HTML Document Standards
- `<!DOCTYPE html>`
- `<html></html>`
- Head : `<head></head>`
    - Title : `<title></title>`
- Link : `<a href="https://www.wikipedia.org/">This Is A Link To Wikipedia</a>`
    - Opening Links in a New Window : `target="_blank"`
    - Linking At Will
    ``` html
    <a href="https://en.wikipedia.org/wiki/Opuntia" target="_blank"><img src="https://www.Prickly_Pear_Closeup.jpg" alt="A red prickly pear fruit"/></a>
    ```
- Linking to the same page : `<a href="#top">Top</a>`
- Recommends 2 spaces of indentation when writing HTML code
- Comment `<!-- comment -->`
