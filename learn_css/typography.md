### Typography
- font-family: Garamond;
- font-weight: bold/normal;
    ``` css
    /*  numeric scale ranging from 100 to 900 */
    font-weitght: 400 /* default */
    font-weitght: 700 /* bold */
    font-weitght: 300 /* light */
    ```
- font-style: italic/normal;
---
- word-spacing: 0.3em;
    - Note that it’s good to use em values in this case because em is dynamic
- letter-spacing: 0.3em;
- text-transform: uppercase/lowercase;
    - [Letter Case Wikipedia](https://en.wikipedia.org/wiki/Letter_case)
- text-align: left/center/right;
----
- line-height: 1.4;
    - **unitless ratio value** : This number is an absolute value that will compute the line height as a ratio of the font size.
![](https://content.codecademy.com/courses/updated_images/htmlcss1-diagram__leading_updated_1-01.svg)

- serif;sans-serif;
![](https://content.codecademy.com/courses/web-101/htmlcss1-diagram__fontanatomy.svg)
- Fallback Fonts
    ``` css
    /* Use the Garamond font for all <h1> elements on the web page.
    If Garamond is not available, use the Times font.
    If Garamond and Times are not available, use any serif font pre-installed on the user’s computer. */
    h1 {
      font-family: "Garamond", "Times", serif;
    }
    ```
----
- Linging Fonts
    ``` css
    <head>
      <link href="https://fonts.googleapis.com/css?family=Droid%20Serif:400,700,700i|Playfair%20Display:400,700,900i" rel="stylesheet">
    </head>    
    ```
- @font-face{}
    ``` css
        /* local font or google font*/
        @font-face {
          font-family: "Glegoo";
          src: url(../fonts/Glegoo-Regular.ttf) format('truetype');
        }
    ```