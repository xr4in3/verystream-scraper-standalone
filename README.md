# Verystream Scraper

[![Build](https://travis-ci.org/MatejTuray/verystream-scraper-standalone.svg?branch=master)]
[![npm version](https://badge.fury.io/js/verystream-scraper-standalone.svg)](https://www.npmjs.com/package/verystream-scraper-standalone)
[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
[![Downloads](https://img.shields.io/npm/dt/verystream-scraper-standalone.svg)](https://npmjs.org/package/verystream-scraper-standalone)

A scraper for [Verystream](https://verystream.com/).

This package is NOT YET part of the [SourceScraper-Project](https://github.com/OpenByteDev/SourceScraper).

Only a standalone module.


## Getting Started
### Installation
```bash
$ npm i verystream-scraper-standalone
```


### Usage

```js
const { VerystreamScraper } = require('verystream-scraper-standalone');

(async () => {
    const url = 'some url';
    const scrap = await new VerystreamScraper().scrap(url);
    if (scrap.success)
        console.log(scrap.data.sources);
})();
```


