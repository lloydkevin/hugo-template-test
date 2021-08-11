# Building a Hugo Theme from scratch

## Getting Started

- Assume base Hugo installation
- `git new site mySite` then `git init`
- add "public/" to gitignore
- Clone theme then delete `.git` folder (Want to own these files now, since they might change from under you) (or use gitmodule? haven't tried that yet)
  - `git clone https://github.com/vimux/blank`

## Start Theming

- Prep HTML template (possibly add to repo so you have original source)
- Copy static assets over to `static` folder.
- Add place holder content files for various pages:
  - Add home page - `hugo new _index.md`
  - Add other index pages - `hugo new blog/_index.md`
  - Add normal pages -  `hugo new about.md`

### Initial Layout

Edit `baseof.html` to match structure from `index.html` or `about.html`.  Everything around `body` tags.

It might be better to user a *normal* page for this initial layout. Tip: do a `diff` between `index.html` and `page.html` to look for structural differences. This may guide how you structure the initial template.

Look for structures that match the Hugo partials: *header, footer, main*. Take note of how *main* differs in the different page templates.

Use lessons to build `single.html`



### Styling Menu

- Add menu items to config file. Make sure to add `weight` field.
- Style menu in navigation [section](https://gohugo.io/templates/menu-templates/)

## Resources

- [Blank Starter Theme](https://themes.gohugo.io/themes/blank/)
- [TOML to YAML converter](https://www.convertsimple.com/convert-toml-to-yaml)
- Markdown Editing - Typora
