# altcoins

[![Build Status](https://travis-ci.org/altcoins/altcoins.github.io.svg)](https://travis-ci.org/altcoins/altcoins.github.io)

A website for discovering alternate cryptocurrencies.

There are a lot of cryptocurrencies out there, but finding out how each of them
is different from the rest is difficult. What is the mining algorithm? What is
the starting difficulty? How many coins will there be? Is this currency a scam?
These are just a few of the questions you need to ask yourself when looking into
a cryptocurrency. This site aims to facilitate your search for answers.

## Running

``` bash
$ git clone https://github.com/altcoins/altcoins.github.io
$ cd altcoins.github.io
$ npm install
$ npm run build
```

The built site will be found in the root directory (GitHub pages requires this).
You can now preview the site with your favorite static web server.

## Adding a cryptocurrency

Cryptocurrencies sit in the `contents/currencies` folder as Markdown files. Each
cryptocurrency has YAML front matter describing the cryptocurrency's properties.
The body of the Markdown file should be a brief description of the currency. The
available metadata fields are:

  - `name` - The name of the currency
  - `tag` - The short code of the currency (like "USD" for the US Dollar)
  - `algorithm` - The mining algorithm of the currency
  - `proof-of-work` - Whether mining is based off proof of work or not
  - `proof-of-stale` - Whether mining is based off proof of stake or not
  - `coins-per-block` - Coins awarded per block
  - `max-coins` - Maximum number of coins the network will ever have