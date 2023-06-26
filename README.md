# Total Computer Care


![Deployment Status](https://github.com/totalcomputercare/website/actions/workflows/jekyll.yml/badge.svg)


[![TCC Logo](img/TCC-logo-full.png)](https://www.totalcomputercare.com.au/)


## Development

```shell
# Checkout repository
git clone git@github.com:totalcomputercare/website.git tcc-website
cd tcc-website
```

```shell
# Build locally 
bundle install
bundle exec jekyll build
```

```shell
# Run the development server
bundle exec jekyll serve
```

### Folder structure

This site uses `Jekyll` to build static pages. Below is a summary of the directory structure

| Name          | Description                                                                              |
|---------------|------------------------------------------------------------------------------------------|
| _layouts      | Contains the default site layout (`default.html`) as well as a helper for minifying HTML |
| _pages        | Contains content for each specific page                                                  |
| _scss         | Contains the partial (S)CSS files                                                        |
| css/site.scss | Main CSS file, use `@import` to bundle the files located in `_scss`                      |
| img/          | Image files for the site                                                                 |  
| _config.yml   | Site configuration file for company-specific values                                      |

### Adding a new page
1. Create a file in `_pages` using the name of the new page (_e.g._ `mypage.html`)
2. Update the header links in `_layouts/default.html`

### Adding a new partial CSS file
1. Create a new file in `_scss` using a descriptive name
2. Add a new `@import` line to `_css/site.css`
