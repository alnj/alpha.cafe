# https://alpha.cafe

![Latest screenshot.](./img/screenshot.png)

Old school fansite for the manga **Yokohama Kaidashi Kikou**. 

#### Borrows elements from late-00s websites:

- Compact design using small text and minimal empty space between elements.
- Narrow max width.
- Emphasis on text over slogans, titles, and images.

This is both purposeful nostalgia and genuine personal preference. 

#### Modern webdesign is still used, e.g.:

- CSS3 properties such as box-shadow, border-radius, transition, and even flexbox.
- CSS functions (var(), calc(), rgba(), linear-gradient()...)
- Fonts.
- Full responsiveness using media queries.
- Webm.
- SCSS.
- HTML5 with semantic elements.

Principles kept in mind:

### Loading times
- Fast loading time is crucial for user experience. Assets are compressed as much as possible.
- Home page is only **320KB** as measured by Lighthouse -- includes images, fonts, stylesheets, thumbnails, etc. 
- Fullsize animations (loaded individually and on demand only) total 360KB. 
- Stylesheet written to have minimal/no layout shift during load time.
- No Flash of Unstyled Text. Flash of Invisible Text softened by using a fade-in animation.

### Clean code
- Simple HTML with emphasis on separation of concerns.
- Meaningless non-semantic markup such as "wrapper" elements must be employed as a last resort.
- Amply commented stylesheet easily maintainable by third parties.
- Elements higher on the page are higher in the stylesheet. Properties are sorted alphabetically. 
- Minimize repetition and maximize themability using variables.

### Appealing prose
- Simple vocabulary and concise phrasing.
- Staying interesting is more important than being comprehensive. 
- Thematic sections must follow crisp headings so users can easily find information relevant to them. 
- Emphasize key words and phrases(?)

### CSS full-size image viewer
- Thumbnails can be enlarged with a click. The full version appears centered above an overlay and can be closed by clicking anywhere.
  - Achieved ~~without JS by wrapping the thumbnail in a checkbox label~~ with JS because I decided to stop being cute and just do it the normal, boring way.
- Before thumbnails are loaded, a nice CSS-only loading animation shows in their stead.

# TODO
More content is to come. Code-wise, I might turn the website into a Single Page Application. (In particular, this would greatly improve UX by not interrupting the background music on page change.)
