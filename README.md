# Hugo Serifed Theme

> **Note:** This is a fork of the [Hugo Serif Theme](https://github.com/zerostaticthemes/hugo-serif-theme) by [Zerostatic Themes](https://www.zerostatic.io/).  
> The original project is MIT licensed (binding). While the MIT license permits reuse, redistribution, and modification, the author has requested in the README that ports should not be made without permission and that the theme should not be re-sold as your own (non-binding).  
> Hence, there is a tension between the permissive legal license and the author’s personal requests.  
> Out of respect for the author, this fork (`hugo-serifed-theme`) is maintained only for **personal/client use and long-term preservation**. It is **not intended to be redistributed, re-sold, or marketed as an original work**.  
> If you want the most up-to-date version or to support the original developer, please visit the [original repo](https://github.com/zerostaticthemes/hugo-serif-theme).


Serif is a modern business theme for Hugo. It contains multiple content types and pages. The theme is fully responsive, blazing fast and artfully illustrated.

[Live Demo](https://hugo-serif.netlify.app/) |  
[Zerostatic Themes](https://www.zerostatic.io/)

![Hugo Serif Theme screenshot](https://www.zerostatic.io/theme/hugo-serif/hugo-serif-screenshot.png)

## Features

**Content Types**

- Services (Markdown)
- Team (Markdown)
- Features (Data)

**CSS**

- SCSS (Hugo Pipelines)
- Fully Responsive design
- Bootstrap 4 grid and media queries only
- Uncomment `@import 'bootstrap/bootstrap';` in `style.scss` to use the entire Bootstrap framework
- Configure Google fonts from `config.toml`
- Configure primary theme colors from `config.toml`
- Examples of using Params from the `config.toml` as SCSS variables

**Speed**

- 100/100 Google Lighthouse speed score
- Under 50KB without images or 80KB with images and illustrations ⚡
- No jQuery, only a tiny bit of vanilla Javascript for the mobile menu.

**SEO**

- 100/100 Google Lighthouse SEO score
- 100/100 Google Lighthouse accessibility score
- Configure Google Analytics in `config.toml`
- Configure Google Analytics using env variable `HUGO_GOOGLE_ANALYTICS_ID` compatible with Netlify.
- Configure meta tags and OG meta tags for the homepage in `config.toml`
- Override any meta tags on a per page basis
- Semantic HTML document structure

**Menu**

- Responsive menu managed in `config.toml`
- Animated hamburger menu on mobile

**Content**

- Robust example content included
- Royalty free illustrations included

**Code**

- No hardcoded content in the layouts
- Plenty of examples of using `range` and `where` to loop over various sections/content types
- Examples of `range` by Param
- Examples of using data content _(`data/contact.yaml` and `data/features.json`)_
- Example of passing .Site . (context) and custom variables to partials - see `layouts/page/contact.html` - `{{ partial "call.html" (dict "site" .Site "context" . "show_button" "false") }}`
- Examples of injecting javascript files on a per page basis (see `services/single.html`)
- Set `body` classes from individual layouts - useful for CSS styling.
- Example of using Hugo custom `layout` for the contact page

## Installation

**1. Install Hugo**

To use this theme you will first need to have Hugo installed. Please follow the official [installation guide](https://gohugo.io/getting-started/installing/)

⚠️ **Note:** Check your Hugo version - **Hugo Extended** is required!

This theme uses [Hugo Pipes](https://gohugo.io/hugo-pipes/scss-sass/) to compile SCSS and minify assets which means if you not using the Hugo extended version this theme will not work. To check your version of Hugo, run `hugo version`. Make sure you see **/extended** after the version number.

**2. Create a new Hugo site**

```bash
hugo new site mynewsite
```

**3. Install the theme**

Clone this fork into your site’s themes folder:

```bash
cd mynewsite
git clone https://github.com/faisaldarbar/hugo-serifed-theme.git themes/hugo-serifed-theme
```

**4. Copy the example content**

```bash
cp -a themes/hugo-serifed-theme/exampleSite/. .
```

**5. Run Hugo**

```bash
hugo server
```

Now open [http://localhost:1313](http://localhost:1313).

## Configuring Theme

### Logo

Edit the logo in `config.toml`:

```toml
[params.logo]
mobile = "images/logo/logo-mobile.svg"
mobile_height = "36px"
desktop = "images/logo/logo.svg"
desktop_height = "36px"
alt = "Serif - A Hugo Business Theme"
```

### Fonts, Colors, Images, Google Analytics, Meta Tags

See original documentation in `config.toml` and theme docs.

## License

MIT © [Zerostatic Themes](https://www.zerostatic.io/)

See [LICENSE](./LICENSE).

## Credits

- Original theme: [Hugo Serif](https://github.com/zerostaticthemes/hugo-serif-theme) by [Zerostatic Themes](https://www.zerostatic.io/)
- Illustrations by [Icons8](https://icons8.com/illustrations/style--pixeltrue)
- Stock images by [Unsplash](https://unsplash.com/)
- Feature icons by [Noun Project](https://thenounproject.com/)
