bridgebeam.design

The Bridgebeam website is built using the Hugo Static Site Generator. To edit the website locally, we have to install Hugo Extended version and NPM/NodeJS (latest version preferrable).

## Overview

Hugo is a static HTML and CSS website generator written in Go. It is optimized for speed, ease of use, and configurability. Hugo takes a directory with content and templates and renders them into a full HTML website.

Hugo relies on Markdown files with front matter for metadata, and you can run Hugo from any directory. This works well for shared hosts and other systems where you don’t have a privileged account.

Hugo renders a typical website of moderate size in a fraction of a second. A good rule of thumb is that each piece of content renders in around 1 millisecond.

## How to install

If you want to use Hugo as your site generator, simply install the Hugo binaries. Use the [installation instructions in the Hugo documentation](https://gohugo.io/getting-started/installing/).

You can install NodeJS/NPM via their [official website](https://nodejs.org/en/download/), or via your local package manager if you're using a *nix operating system.

## Local testing

After installing NodeJS, we have to run the following command inside the root path of the website.

`npm install`

This will install the required modules we use to tree-shake the CSS files and make them smaller, greatly reducing loading size and time.

Afterwards, we have to run Hugo with the following command.

`hugo server --environment production`

The `--environment` argument is necessary for us to be able to render the content in the same way that the public version would come out to be.

With this we're ready to start editing the files.