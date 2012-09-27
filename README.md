jQuery Selector Cache
=============

Cache your selectors, without messy code.

Installation
-------

1. Include the /src/jquery.sc.js file.

Usage
------------

### Overview
Instead of `$('div')` use `$$('div')`

### Get
`$$('div')`

The next time you call `$$('div')` it will be fetched from the cache.

### Clear
`$$('div', 'clear')`

Invalidates the cache. The next time you call `$$('div')` It will return fresh results.

### Fresh
`$$('div', 'fresh')`

Shortcut for doing `$$('div', 'clear')` `$$('div')`

Benchmarks
------------

    No cache: 444ms
    Selector Cache plugin: 3ms
    Storing results in variables: 2ms