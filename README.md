# WSTG Page on the OWASP Website

This repository contains the files that build the Web Security Testing Guide (WSTG) Project's page on the main OWASP website. The page can be found at: https://owasp.org/www-project-web-security-testing-guide/

Documentation explaining the files in this repo can be found at: https://owasp.org/migration

## Contributions

Any contributions to the guide itself should be made via the [guide's project repo](https://github.com/OWASP/wstg), using a pull request. (No one outside the project leadership or foundation automation should be pushing directly to either repo.)

## Getting Started

To set up a local development environment for this [Jekyll](https://jekyllrb.com/docs/installation/ubuntu/) site:

1. Install Jekyll and its required dependencies for your operating system. See [Installation](https://jekyllrb.com/docs/installation/).
2. Clone this repository, for example: 

    `git clone git@github.com:OWASP/www-project-web-security-testing-guide.git www-wstg`

3. Change into the repository directory and install dependencies with:

    `cd www-wstg && bundle install`

4. Serve the site to view it locally by running:

    `bundle exec jekyll serve`
