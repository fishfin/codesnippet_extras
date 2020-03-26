# [[fishfin] codesnippet_extras](https://github.com/fishfin/codesnippet_extras)

> ```#drupal8``` ```#drupal9``` ```#module```

This Drupal 8 custom module adds additional languages and styles from [highlightjs](https://highlightjs.org) library to [CKEditor CodeSnippet](https://www.drupal.org/project/codesnippet) plugin.

This module should work with Drupal 9 without any changes (not tested - yet).

### Installation

To install this package using composer, copy ```composer.codesnippet_extras.json``` to root of your Drupal install (or a directory in it, viz. ```composer```), and from the root ```composer.json```, ```include``` or ```require``` it using the ```wikimedia/composer-merge-plugin``` package. Sample is given below:

**Root ```composer.json```:**

```json
{
  "require": {
    "wikimedia/composer-merge-plugin": "^1.4"
  },
  "extra": {
    "merge-plugin": {
      "include": [
        "composer/composer.codesnippet_extras.json"
      ],
      "require": [],
      "recurse": true,
      "replace": false,
      "ignore-duplicates": false,
      "merge-dev": true,
      "merge-extra": true,
      "merge-extra-deep": true,
      "merge-scripts": false
    }
  }
}
```