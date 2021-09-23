# revealjs (development version)

- Add `toc` and `toc_depth` argument in `revealjs_presentation()` as with `rmarkdown::html_document()`. Set `toc = TRUE` to create a slide after the title slide containing a Table Of Content. `toc_depth = 3` by default (as Pandoc) - its value must be adjusted with `slide_level` is you do not get the desired result, depending if you are using 2D slides or not.

- `smart` argument has been removed from `revealjs_presentation()` has no more used by **rmarkdown**. `smart = TRUE` is still the default. If you need to deactivate, use `md_extensions = "-smart"`.

- Add `title-slide` id on the auto generated title slide to ease the styling using CSS.

- Support more Pandoc's variable in `revealjs_presentation()` as documented in Pandoc for HTML slides:
* `background-image` to customize the option `parallaxBackgroundImage`. This duplicates the variable `parallaxBackgroundImage` which still get precedence.
* `institute` to provide another line in title slide between author and date
* `toc-title` to provide a Title above the toc when `toc = TRUE`

- Fix template to add the necessary CSS to format [columns layout](https://pandoc.org/MANUAL.html#columns) and other Pandoc's features (thanks, @atusy, #82).

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
