# The ARCA theme


*ARCA theme is a Jekyll theme for GitHub Pages. You can [preview the theme to see what it looks like](https://arca-dpss.github.io/ARCA-ghpages/), or even [use it today](#usage).*

<img src="thumbnail.png" width="200"/>

This theme is based on [Cayman theme](https://github.com/pages-themes/cayman) and [Leap-day theme](https://github.com/pages-themes/leap-day).

## Usage

To use the ARCA theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    remote_theme: arca-dpss/ARCA-ghpages
    ```

## Customizing

To know more about customizing the template see [Cayman doucmentation](https://github.com/pages-themes/cayman).


## Configuration variables

ARCA will respect the following variables, if set in your site's `index.md`:

```yml
---
course_title: Title of the course
author_name: Author Name
---
```

Additionally, you may choose to set the following optional variables in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
show_downloads: ["true" or "false" (unquoted) to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]
```

### Overriding GitHub-generated URLs

Templates often rely on URLs supplied by GitHub such as links to your repository or links to download your project. If you'd like to override one or more default URLs:

1. Look at [the template source](https://github.com/arca-dpss/ARCA-ghpages/blob/master/_layouts/default.html) to determine the name of the variable. It will be in the form of `{{ site.github.zip_url }}`.
2. Specify the URL that you'd like the template to use in your site's `_config.yml`. For example, if the variable was `site.github.url`, you'd add the following:
    ```yml
    github:
      zip_url: http://example.com/download.zip
      another_url: another value
    ```
3. When your site is built, Jekyll will use the URL you specified, rather than the default one provided by GitHub.

*Note: You must remove the `site.` prefix, and each variable name (after the `github.`) should be indent with two space below `github:`.*

For more information, see [the Jekyll variables documentation](https://jekyllrb.com/docs/variables/).


