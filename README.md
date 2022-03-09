# Documentation

## Fonts
- Lato for Headings
- Avenir for Body Text
- Playfair Display for Quotes inside the articles on resource page

### Font sizes
H1 `45px`; H2 `26px`; H3 `22px`; H4 `20px`; Menu Items/Body Text/Overline Text `16px`; Button Text `14px`

### Colors
- primary: #282828
- secondary: #454545
- accent: #004970

### Image Sizes 

Icons `.svg` format; Illustrations `.svg` format; In file Image(s) `.jpg` or  `.png` format

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

```
Please note while placing images in `.md` files, make sure to put `{{site.baseurl}}` before the image source.

For example:

![Inficold]({{site.baseurl}}images/company/Img1.JPG)

```


---


## _resource

### Widgets 
- `{% include cta.html %}` For CTA
- `{% include faq.html %}` For FAQ
- `{% include second-faq.html %}` For second FAQ block
<br>
**For Reusable layouts, please find the code snippets in** `code-snippets.md`

### Liquid Tags in Front Matter (Explanation)

Boolean input(true/false)
- `promoted: ` or `show-page: ` To display the page or not entirely on `resources` page
- `show-faq: ` To display the faq widget or not
- `show-second-faq: ` To display the second-faq widget or not
- `show-cta: ` To display the cta widget or not
- `show-cover-image: ` To display the cover image or not

CONTENT
- `title: ` Main title of the page
- `image: ` For the main icon shown with the article on `resources` page. Here you need to place the icon link from assets folder
- `headline: ` This is the over line text displayed above your main title/heading on the Resources page
- `category: ` What filter category you want to showcase this page in?

CTA TAGS
- `cta-heading: ` title of the cta
- `cta-description: ` content within the cta box
- `cta-button-text: ` what will the button say?
- `cta-button-url: ` put the link where the user will be re-directed when they click on the button

FAQ TAGS
- `faq-heading-1: ` and `faq-heading-2: `  Add headings to the faq sections here
- `questions: ` and `questions-block2: ` Write the questions to be displayed in FAQ 1 and FAQ 2
- `answers: ` and `answers-block2: ` Write the answers to be displayed for questions in FAQ 1 and FAQ 2

COVER IMAGE TAGS
- `cover-image: ` Here you need to place the image link for the cover
- `cover-quote: ` The quote you want to place on the cover-image
- `quote-author: ` Name of the author who said the quote
- `quote-author-designation: ` Designation of the author
- `quote-author-image: ` Image of the author
- `author-linkedinurl: ` Here you need to place the linkedIn url of the author

---


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
