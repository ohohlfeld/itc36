## Setup

1. Clone repository or use the "Use this template" button
2. Open `_config.yml` and adapt variables
3. Replace **TODO**s with custom text


## Running

```sh
$ bundle exec jekyll serve
```
The command outputs an URL under which the site can be reached, usually `http://127.0.0.1:4000/`.
The server regenerates automatically whenever the content changes.

## Github Pages

Github generates the site from the `gh-pages` branch by default.
Therefore, changes in `master` need to be merged over to `gh-pages`.

It is important that `baseurl` in `_config.yml` is empty. Github will automatically fill in the correct string, according to which domain is used.
E.g. when hosting on Github with default `user.github.io/project` domain, baseurl will be the project name.

After pushing, it may take a moment for the website to update.


## Custom domain

See also [here](https://help.github.com/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site).

To setup a custom domain:

1. Use the repository settings on Github or manually create a file `CNAME` in the project root of the `gh-pages` branch.

    It contains the domain the site should be available at, e.g. `itc31.itc-conference.org`.

    **Note** (Depending on your workflow): Make sure to merge this CNAME commit back into `master`, so that both branches, `master` and `gh-pages`, are equal. This keeps the git history nice and clean when merging back and forth between `master` and `gh-pages`.

2. Go to [Host Europe](https://sso.hosteurope.de/?app=kis&path=%2F), create a new subdomain CNAME entry for `itc-conference.org`, and link it to `lsinfo3.github.io`.

3. It takes a moment to update and generate the HTTPS certificate.

    After that the site should be available from the respective domain.

4. Create an additional redirect in the `itc-conference` repo, so that the site is accessible using `itc-conference.org/itcXY`. See [here](https://github.com/lsinfo3/itc-conference#redirects) for instructions.

## Links

Since `baseurl` may vary, it is not advised to use bare absolute paths, e.g. `/assets/images/image.png`, but `{{ site.baseurl }}` instead.

Relative paths should be fine.

**Example**:
```Markdown
<img src="{{ site.baseurl }}/assets/images/logo.png">

![]({{ site.baseurl }}/assets/images/logo.png)

[Link]({{ site.baseurl }}/index.html)

[Relative Link](index.html)

<img src="../assets/images/logo.png">
```


## Creating new pages

Create a new markdown file with the following structure and adapt to your needs.
```
---
title: Page Title
menu: top-nav
menu-index: 1
---

Page content here
```

| Key        | Meaning             |
|------------|---------------------|
| title      | Page title          |
| menu       | The navigation menu the page will be listed in. `top-nav` for main menu, `footer-nav` for footer menu. Leave out this key for no entry. |
| menu-index | Position in menu (only needed when `menu` is set) |



## Adding news entries

Create a new markdown file in the `_posts` directory with the filename `YYYY-MM-DD-titel.md`, where YYYY, MM, DD stands for year, month, and day.
`title` and `author` need to be defined in the front-matter of each post:

```
---
author: ITC
title: Example Title
---

Post content
```

The news page will be generated automatically from all posts.

## Sidebar

Changes to sidebar content, except "Important Dates" and "Sponsors", need to be added manually in `_layouts/default.html`.

For "Important Dates" and "Sponsors", there's a respective file in `_includes`. The "Contact Us" section is generated automatically using the `conference-mail` variable defined in `_config.yml`.
