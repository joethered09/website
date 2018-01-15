# Data Together Website

<!-- Repo Badges for: Github Project, Slack, License-->

[![GitHub](https://img.shields.io/badge/project-Data_Together-487b57.svg?style=flat-square)](http://github.com/datatogether)
[![Slack](https://img.shields.io/badge/slack-Archivers-b44e88.svg?style=flat-square)](https://archivers-slack.herokuapp.com/)
[![License](https://img.shields.io/github/license/datatogether/website.svg?style=flat-square)](./LICENSE)

A website to introduce the Data Together project, describing our collective commitment to support the development of a decentralized web that aggregates and preserves the public record, with attention to provenance and trustworthiness of our data. Built with [Hugo](https://gohugo.io/), a fast and modern static site generator written in Go, and [Gulp](https://gulpjs.com/), an automated task runner.

## License

<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">The Data Together Website</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

## Getting Involved

We would love involvement from more people! If you notice any errors or would like to submit changes, please see our [Contributing Guidelines](./.github/CONTRIBUTING.md).

We use GitHub issues for [tracking bugs and feature requests](https://github.com/datatogether/website/issues) and Pull Requests (PRs) for [submitting changes](https://github.com/datatogether/website/pulls).

## Structure

- `config.toml`, site-wide configuration options and settings
- `content/`, markdown files for each page (`.md`)
- `themes/datatogether`, website format (`layouts/`) and styling via compiled sass (`src/`)

## Development

1. Install Hugo and Gulp

    To get started, follow the [Hugo install instructions](https://gohugo.io/getting-started) and [Gulp install instructions](https://gulpjs.com/).

1. Clone this repo and `cd` into the directory

    ```
    $ git clone git@github.com:datatogether/website.git
    $ cd website
    ```

1. Make Changes and Test Locally

    Using your favourite text editor to make changes. If you are new to Hugo, you may want to read about [usage basics](https://gohugo.io/getting-started/usage/) and the [directory structure](https://gohugo.io/getting-started/directory-structure/).

    Hugo also includes a development server so you can view your changes as you go. Spin it up with the following command:

    ```
    $ hugo serve
    ```

    For any changes to the sass style, run `gulp styles` from `themes/datatogether/src/` to recompile `.scss` files into `.css`.

1. Rebuild and Commit

    Run `hugo` before adding changes to a git commit.


### Dependencies

- [bootstrap-sass](https://github.com/twbs/bootstrap-sass)
- [normalize.css](https://github.com/necolas/normalize.css)

## Deployment

[datatogether.org](https://datatogether.org/) is manually deployed over IPFS ([the InterPlanetary File System](https://ipfs.io/)) using IPNS (the Inter-Planetary Naming System), you can also view the site via an IPFS gateway at [ipfs.io/ipns/datatogether.org](https://ipfs.io/ipns/datatogether.org/).
