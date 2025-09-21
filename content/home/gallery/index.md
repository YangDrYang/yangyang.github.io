+++
# Gallery section using the Blank widget and Gallery element (shortcode).
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 120  # Order that this section will appear.

title = "Gallery"
subtitle = "Photos with my students"

[[gallery_item]]
album = "gallery"
image = "user.jpg"
caption = "Yang at UNSW"

[[gallery_item]]
album = "gallery"
image = "user-2.jpg"
caption = "LAB session"

[[gallery_item]]
album = "gallery"
image = "user-full.jpg"
caption = "Seminar talk"

[[gallery_item]]
album = "gallery"
image = "user-full-2.jpg"
caption = "Team meeting"

[[gallery_item]]
album = "gallery"
image = "geo.jpg"
caption = "Sydney skyline"
+++

Here are some photos with my colleagues and students. 

{{< gallery_slider album="gallery" interval="5000" per="2" >}}
