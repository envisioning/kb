# Envisioning's Knowledge Base

It is running under Raneto (NodeJS)

## Installing & Running it locally

1. Clone the repo to your computer
2. Make sure you have `npm` & `gulp` installed. If you have it, skip to step `6`
3. Install `Home Brew` on your Mac, by opening the console and typing `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
4. Install `node` via Brew: `brew install node`
5. Install `grunt` via node: `npm install --global gulp-cli`
6. Browse to the project dir and do `npm install`
7. Start the server by running `npm start`
8. Your server is running at `http://localhost:3000/`

## Adding content

Pages are generated via Markdown files placed inside `/content`. Each folder creates a section and each markdown inside the folder creates an article.

Articles should have a specific markdown header with Title, Description and Sort Order (optional, otherwise alphabetically ordered).

```markdown
/*
Title: Why technology?
Description: Envisioning's Knowledge base
Sort: 1
*/
```

Folders can be sorted with a `sort` file and an integer as content.

### Images

You should save images inside `/themes/default/public/images` and link them with the relative path in markdown: `![](%image_url%/readiness02.jpg)`.


## Templating 

Theme is inside `/themes/default`. Basic files are `layout.html` & `page.html`