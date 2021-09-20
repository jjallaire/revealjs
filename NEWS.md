# revealjs (development version)

- Fix an issue with some configurations keys for chalkboard plugin - multiple value are now correctly passed to Pandoc's template (thanks, @grayknight2, @atusy, #62, #88).

- Fix issues with quoting of options when passed as variables to Pandoc. This was caused by a change in Pandoc 2.14.0.3 which now sets some default value for reveal.js options (thanks, @iain-palmer, #72).

- Add `md_extensions` argument in `revealjs_presentation()` (thanks, @atusy, #75).

# revealjs 0.9

- Add support for the menu plugin

- Correct handling of pdf css for self_contained document

- Remove _html5shiv.js_ from template


# revealjs 0.8

- Add support for the chalkboard plugin


# revealjs 0.7

- Update to _reveal.js_ 3.3

- Push slide changes to browser history

- Respect `slide_level` option

- Support for zoom, search, and notes _reveal.js_ plugins

- Ability to specify `slideNumber` reveal_option as either string or boolean


# revealjs 0.6

- Fix issue with missing embedded fonts for beige, league, and 
  solarized themes.


# revealjs 0.5

- Initial release to CRAN
