heatmaply 0.3.2 (2016-05-26)
==============================

### ANNOUNCMENTS
* heatmaply 0.3.2 - first CRAN release!

### BUG FIXES
* http -> https

heatmaply 0.3.1 (2016-05-26)
==============================
### BUG FIXES
* fix minor typos.

heatmaply 0.3.0 (2016-05-25)
==============================


### NEW FEATURES
* heatmaply
  * Now works with Rowv=F and Colv=F (by introducing a new un-exported function: heatmap_subplot_from_ggplotly)
  * Remove space between the heatmap and dendrograms (via: coord_cartesian(expand = FALSE)  and coord_flip(expand = FALSE))
  * Added the margin parameter (to control the distance between the heatmap and the dendrograms.)
  * Added row_text_angle and column_text_angle (with srtRow and srtCol for backward compatibility with gplots::heatmap.2). Fix #3

### BUG FIXES
* fix #2 : Error: Don't know how to add scale_fill_gradient_fun to a plot
  by moving "scale_fill_gradient_fun" after "..." (I may change this parameter's name later)


### VIGNETTE
* heatmaply now has a basic vignette.


heatmaply 0.2.1 (2016-05-23)
==============================

### BUG FIXES
* fix various import issues that caused warnings with devtools::check()


heatmaply 0.2.0 (2016-05-23)
==============================
### NEW FEATURES
* More control over colors in heatmaply via the new parameters: colours, limits, na.value, and scale_colour_gradient_fun.
* first attempts at row_dend_left (although this is not yet working.)

### BUG FIXES
* dendrograms are now presented without axes text.
* passing scale (= "row" or "column") works again.


heatmaply 0.1.0 (2016-05-14)
==============================

* First (very rough) version. It has a minimal working example, as well as MANY things to fix/tweak/adjust.




TODO:
==============================
* add bars for extra categories
* remove hover information from dendrograms
* remove unneeded code from d3heatmap
* add many options for controlling the heatmap "as it should be"
* implement all relevant options streight to heatmaply.

* write a post!
