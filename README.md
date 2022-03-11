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

Icons `.svg` format; Illustrations `.svg` format; In-file Image(s) `.jpg` or  `.png` format

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
    - Circular shape; Background color: white; Drop shadow: Blur 10; Y 5; #263238 Opacity 5%
    - Icon color; Linear gradient: Color1 rgb(69,69,69) Opacity 100% | Color2 rgb(0,73,112) Opacity 100%

- Cover images for Articles in Resource page;
    - minimum size 2000x500px `less than 1mb; .jpg/.png`
    - to ensure maximum readability of the quote please put a black overlay of around 30% before uploading the image to the `cover` folder.

- Authors' images for quotes in articles;
    - minimum size 68x68px `.svg`
    - Circular shape
    - White outer stroke with inner shadow (present - optional); can also be replaced with a white drop shadow

---


### Markdown and CSS Guides
- [.md Syntax Guide](https://www.markdownguide.org/basic-syntax/)
- CSS Syntax Guides
    [w3schools](https://www.w3schools.com/css/default.asp)
    [tutorialspoint](https://www.tutorialspoint.com/css/index.htm)

```
Please note while placing images in `.md` files, make sure to put `{{site.baseurl}}` before the image source.

For example:

![Inficold]({{site.baseurl}}/images/company/Img1.JPG)

```


## Global 
- To activate google analytics, update google_analytics_id in seo.yml
- To publish, update `baseurl` and `permalink` in `_config.yml`
- Global stylesheet can be found in `assets/css/style.css`
- Logo can be updated in `_congig.yml`
- Social profiles can be updated in `data/social.json`
- Menu can be updated in `data/menus.yml`
- Styling sheets for components like footer, social icons, header etc. can be found under `_sass/components`


## Home

This is the main page of the website.

- Associated Page `index.md`
- The base layout for this page can be found in `_layouts/home.html`
- The CSS styling sheet for this page can be found in `_sass/pages/page-home.scss`
- Illustrations used on home page can be found in `images/illustrations`

---


## Team

This is the main page which displays all the team members present in `team` folder.

- Associated Page `team.md`
- The base layout for this page can be found in `_layouts/teams.html`
- The CSS styling sheet for this page can be found in `_sass/pages/page-teams.scss`
- Team members' photographs can be found in `images/team`

## _team

This folder contains all the markdown files for the team members being displayed on `Team` page.

- The base layout for each team member can be found in `_layouts/team.html`
- The CSS styling sheet for this folder can be found in `_sass/pages/page-team.scss`
- Additonal team member can be added in this `_team` folder

### Liquid Tags in Front Matter (Explanation)

- `title: ` Here you'll enter the name of the team member
- `image: ` Add photograph of the member here
- `jobtitle: ` Add their job title here
- `linkedinurl: ` Add linkedIn url here
- `twitterurl: ` Add twitter url here
- `twitterUsername: ` Add twitter username with @ here
- `category: ` What filter category you want to showcase this page within?


---


## Portfolio

This is the main page which displays all the companies present in `portfolio` folder.

- Associated Page `portfolio.md`
- The base layout for this page can be found in `_layouts/portfolios.html`
- The CSS styling sheet for this page can be found in `_sass/pages/page-portfolios.scss`
- You can edit the categories used in filters in  `_layouts/portfolios.html`
- Company logos can be found in `images/portfolio`
- You can add images to use within these portfolio pages in `images/company`

## _portfolio

This folder contains all the markdown files for the companies being displayed on `Portfolios` page.

- The base layout for each portfolio page can be found in `_layouts/portfolio.html`
- The CSS styling sheet for this folder can be found in `_sass/pages/page-portfolio.scss`
- Additonal company portfolio can be added in this `_portfolio` folder

### Liquid Tags in Front Matter (Explanation)

- `title: ` Main title of the page. Here you'll enter the name of the company
- `image: ` Add company's logo image here
- `tagline: ` Companys' slogan etc.
- `websiteurl: ` Companys' main websites' url
- `category: ` What filter category you want to showcase this page within?


---


## Resources

This is the main page which displays all the articles present in `_resource` folder.

- Associated Page `resource.md`
- The base layout for this page can be found in `_layouts/resources.html`
- Icons used with every article can be found in `images/resource`
- The CSS styling sheet for this page can be found in `_sass/pages/page-resources.scss`
- You can edit the categories used in filters in  `_layouts/resources.html`

## _resource

This folder contains all the markdown files for the articles/pages being displayed on `Resources` page.

- The base layout for each resource page can be found in `_layouts/resource.html`
- New article pages can be added in this folder `_resource`
- The CSS styling sheet for this folder can be found in `_sass/pages/page-resource.scss`
- Cover Images for the articles in reources page can be found in `images/cover`
- Author Images for the quotes in reource articles can be found in `images/author`

### Widgets 
- `{% include cta.html %}` For CTA
- `{% include faq.html %}` For FAQ
- `{% include second-faq.html %}` For second FAQ block
<br>

```
For Reusable layouts (2 column, 3 column, and 1:2 column ), please find the code snippets in `code-snippets.md`
```

### Liquid Tags in Front Matter (Explanation)

Boolean input(true/false)
- `promoted: ` or `show-page: ` To display the page or not on `Resources` page
- `show-faq: ` To display the faq widget or not
- `show-second-faq: ` To display the second-faq widget or not
- `show-cta: ` To display the cta widget or not
- `show-cover-image: ` To display the cover image or not

CONTENT
- `title: ` Main title of the page
- `image: ` For the main icon shown with the article on `resources` page. Here you need to place the icon link from assets folder
- `headline: ` This is the over line text displayed above your main title/heading on the Resources page
- `category: ` What filter category you want to showcase this page within?

CTA TAGS
- `cta-heading: ` title of the cta
- `cta-description: ` content within the cta box
- `cta-button-text: ` what will the button say?
- `cta-button-url: ` put the link where the user will be re-directed when they click on the button

FAQ TAGS
- `faq-heading-1: ` and `faq-heading-2: `  Add headings to the faq sections here
- `questions: ` and `questions-block2: ` Write the questions to be displayed in FAQ 1 and FAQ 2
- `answers: ` and `answers-block2: ` Write the answers to be displayed for questions in FAQ 1 and FAQ 2
- `faqImages11: ` and `faqImages12: ` To add images in the answer blocks of first FAQ 
- `faqImages21: ` and `faqImages22: ` To add images in the answer blocks of second FAQ 

COVER IMAGE TAGS
- `cover-image: ` Here you need to place the image link for the cover
- `cover-quote: ` The quote you want to place on the cover-image
- `quote-author: ` Name of the author who said the quote
- `quote-author-designation: ` Designation of the author
- `quote-author-image: ` Image of the author
- `author-linkedinurl: ` Here you need to place the linkedIn url of the author


---


## Privacy Policy

This page is linked in sub-footer. Associated page `privacy-policy.md`


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


---


### Jekyll's official documentation

- [Jekyll](https://jekyllrb.com/) (official)
- Jekyll theme used - [Serif](https://www.zerostatic.io/theme/hugo-serif/)
