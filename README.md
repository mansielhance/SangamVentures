# Documentation

### Fonts
- Lato for Headings
- Avenir for Body Text
- Playfair Display for Quotes inside the articles on resource page

## Font sizes
- H1 `45px`
- H2 `26px`
- H3 `22px`
- H4 `20px`
- Menu Items/Body Text/Overline Text `16px`
- Button Text `14px`

### Colors
- primary: #282828
- secondary: #454545
- accent: #004970

### Image Sizes 

Icons `.svg` format
Illustrations `.svg` format
In file Image(s) `.jpg` or  `.png` format

`wxh`

- Home Page Illustrations;
    - minimum width up to 1500 - 2000px
    - export in either `.png` or `.svg` 
    - size in `.kb` for optimal loading

- Team Page;
    minimum image size 400x400px

- Portfolio Page;
    - minimum image size 700x400px
    - Outside stroke #004970 Opacity 88%

- Portfolio Internal Pages;
    - images for this can be stored in `images/company` folder
    - please ensure the images are of same size before placing them on the page

- Resource Page Icons;
    - minimum size 68x68px `.svg`
    - Circular shape
    - Drop shadow: Blur 10; Y 5; #263238 Opacity 5%

- Cover images for Articles in Resource page;
    - minimum size 2000x500px `less than 1mb; .jpg/.png`
    - to ensure maximum readability of the quote please put a black overlay of around 30% before uploading the image to the `cover` folder.

- Authors' images for quotes in articles;
    - minimum size 68x68px `.svg`
    - Circular shape
    - White outer stroke with inner shadow (present - optional); can also be replaced with a white drop shadow


---


### Additional Information

- To activate google analytics, update google_analytics_id in `seo.yml`

- Additonal team members can be added in `_team`

- Additonal company portfolio can be added in `_portfolio`

- New articles can be added in `_resource`

- Cover Images for the articles in reources page can be found in `images/cover`

- Author Images for the quotes in reource articles can be found in `images/author`

### External Resources
- [.md Syntax Guide](https://www.markdownguide.org/basic-syntax/)
- CSS Syntax Guides
    [w3schools](https://www.w3schools.com/css/default.asp)
    [tutorialspoint](https://www.tutorialspoint.com/css/index.htm)


---


### _resource

## Widgets 
- `{% include cta.html %}` For CTA
- `{% include faq.html %}` For FAQ
- `{% include second-faq.html %}` For second FAQ block
- `{% include show-2-column.html %}` For 2 column layout

## Liquid Tags in Front Matter (Explanation)

Boolean input(true/false)
`promoted: ` or `show-page: ` To display the page or not entirely on `resources` page
`show-faq: ` To display the faq widget or not
`show-second-faq: ` To display the second-faq widget or not
`show-cta: ` To display the cta widget or not
`show-cover-image: ` To display the cover image or not
`show-2-column-layout: ` To display the second column layout

Content
`image: ` For the main icon shown with the article on `resources` page
`cover-image: ` For the main co

### Testing on local server

To run the website on local server, navigate to the theme directory and run:

```
bundle exec jekyll serve
``` 

To stop the server

```
ctrl+c
``` 

### To publish

Update `baseurl` and `permalink` in `_config.yml` 


### Jekyll's official documentation

- [Jekyll](https://jekyllrb.com/) (official)
- Jekyll theme used - [Serif](https://www.zerostatic.io/theme/hugo-serif/)
