# Changelog

## 3.0.0

- added `Minifier` namespace
- submitted to Packagist to use `composer require pfaciana/tiny-html-minifier` to autoload

## 2.2.0

- Removed experimental feature json-ld as it was too buggy.
- Added option to disable comments.
- Changed regex for removing comments due to reported buggy sometimes. Thanks to [@MuetzeOfficial](https://github.com/MuetzeOfficial) for the suggested fix.
- Added fix for whitespace before doctype. Thanks to [@alpipego](https://github.com/alpipego) for the fix.

## 2.1.0

- Added experimental feature support for minify `<script type="json-ld"></script>`.

## 2.0.0

- A complete rewrite and bump to version 2.
- Inline SVG files are supported and will be minified.
- Custom Elements support (`<my-element>My content</my-element>`).
- The slash of self closing tags are removed from ` />` to `>`.
- Unneeded element data are removed from `style` and `script` tags (` type="text/css"` and ` type="text/javascript"`).
- The minifier is now aware of what's inside `<head></head>` and will minify it without leaving the spaces (except for `style` and `script`).
- Instead of whitelist all allowed elements, it minifies all tags, but skip `textarea`, `code`, `pre` and `script`.
- The code length is reduced from around 300 lines to around 200 lines.

## 1.2.0

- Instead of remove CDATA, it will now be kept.
- Better JSON support.

## 1.1.0

Minor bug fixes

## 1.0.0

Initial release