# README
Repository for XSpec website [xspec.io](https://xspec.io).

The default branch is the `hugo` branch, containing the sources of the actual website.

To run a local version:

* [Install Hugo following their instructions](https://gohugo.io/getting-started/installing/).
* Clone or download this repository from GitHub.
* Checkout the branch `hugo`: `git checkout hugo`
* Install the git submodules: `git submodule update --init --recursive`
* Run `hugo server -D` to get a local version of the website.

To submit updates: create a pull request to the `hugo` branch.

## Background

The website is generated as a static site using [Hugo](https://gohugo.io/). The static site is stored in the `master` branch, and GitHub publishes the static site.