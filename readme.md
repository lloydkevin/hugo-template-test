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

Edit `baseof.html` to match structure from `index.html`. Everything around `body` tags.

## Resources

- [Blank Starter Theme](https://themes.gohugo.io/themes/blank/)
- [TOML to YAML converter](https://www.convertsimple.com/convert-toml-to-yaml)
- Markdown Editing - Typora
