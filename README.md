# Sangam Ventures' Website Documentation

## Base Details

### Fonts
- Lato for Headings
- Avenir for Body Text
- Playfair Display for Quotes inside the articles on resource page

### Colors
- primary: #004970
- primary-dark: #00abbd
- secondary: #8ed8f8

### Image Sizes 
All images/icons used are in either `.jpg` or  `.svg` format as per use case.

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

- Resource Page Icons;
    - minimum size 68x68px `.svg`
    - Circular shape
    - Drop shadow: Blur 10; Y 5; #263238 Opacity 5%

- Cover images for Articles in Resource page;
    - minimum size 2000x500px `less than 1mb; .jpg`
    - please put a black overlay of around 30% before exporting the image to the `cover` folder so that the quote is visible when successfully uploaded.

- Authors' images for quotes in articles;
    - minimum size 68x68px `.svg`
    - Circular shape
    - White outer stroke with inner shadow (present - optional); can also be replaced with a white drop shadow

## Additional Information

- To activate google analytics, update google_analytics_id in `seo.yml`

- Additonal team members can be added in `_team`

- Additonal company portfolio can be added in `_portfolio`

- New articles can be added in `_resource`

- Cover Images for the articles in reources page can be found in `images/cover`

- Author Images for the quotes in reource articles can be found in `images/author`

### Running on local server

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

## Checklist

- [ ] Responsiveness

### Home Page

- [x] How, What, Why linked via anchors
- [x] Pop-up modal for "Join Us" button

### Team Page

- [x] Tile view of team members
- [x] Name, designation, twitter link

### Internal Team Pages

- [x] Name, designation, about
- [x] Links and photograph

### Portfolio Page

- [x] Tile view for the companies
- [ ] Filters

### Internal Portfolio Pages

- [x] Company name, about
- [ ] Photograph, links, works

### Resources Page

- [x] Tile view for articles 
- [ ] Filters

### Internal Article Pages for Resources

- [x] Section for quotes with the person's photo and link to their profile
- [x] Title and Description
- [ ] CTAs to lead to other pages
- [ ] FAQ section


### Jekyll's official documentation

- [Jekyll](https://jekyllrb.com/) (official)
- Jekyll theme used - [Serif](https://www.zerostatic.io/theme/hugo-serif/)
