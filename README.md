# Sangam Ventures' Website Documentation

## Base Details

### Fonts
Lato for Headings
Avenir for Body Text

### Colors
primary: #004970
primary-dark: #00abbd
secondary: #8ed8f8

### Image Sizes 
All images/icons used are in `.svg` format

`wxh`

- Team Page
    minimum image size 400x400px

- Portfolio Page
    minimum image size 700x400px

- Resource Page Icons
    minimum image size 68x68px

## Additional Information

- To activate google analytics, update google_analytics_id in `seo.yml`

- Additonal team members can be added in `_team`

- Additonal company portfolio can be added in `_portfolio`

- New articles can be added in `_resource`

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


### Jekyll's official documentation

- [Jekyll](https://jekyllrb.com/) (official)
- Jekyll theme used - [Serif](https://www.zerostatic.io/theme/hugo-serif/)
