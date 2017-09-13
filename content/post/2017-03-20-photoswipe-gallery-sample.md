---
title: Plot Gallery Sample
subtitle: Making a Gallery
tags: ["statistics", "ggplot2"]
---

The well-known `R` library [ggplot2](http://ggplot2.tidyverse.org/reference/) is very useful to 

{{< gallery caption-effect="fade" >}}
  {{< figure thumb="-thumb" link="/img/gev_comp_v1.jpg" >}}
  {{< figure thumb="-thumb" link="/img/gev3.jpg" caption="Generalized Extreme Value Distribution" >}}
  {{< figure thumb="-thumb" link="/img/post_draws.jpg" caption="Posterior draws from GAM with splines" alt="Smoothing method" >}}
 {{< figure thumb="-thumb" link="/img/violin_density.jpg" caption="Violin and density plots " >}}
{{< /gallery >}}


## Usage
For full details please see the [hugo-easy-gallery GitHub](https://github.com/liwenyip/hugo-easy-gallery/) page. Basic usages from above are:

- Create a gallery with open and close tags `{{</* gallery */>}}` and `{{</* /gallery */>}}`
- `{{</* figure src="image.jpg" */>}}` will use `image.jpg` for thumbnail and lightbox
- `{{</* figure src="thumb.jpg" link="image.jpg" */>}}` will use `thumb.jpg` for thumbnail and `image.jpg` for lightbox
- `{{</* figure thumb="-small" link="image.jpg" */>}}` will use `image-small.jpg` for thumbnail and `image.jpg` for lightbox
- All the [features/parameters](https://gohugo.io/extras/shortcodes) of Hugo's built-in `figure` shortcode work as normal, i.e. src, link, title, caption, class, attr (attribution), attrlink, alt
- `{{</* gallery caption-effect="fade" */>}}` will fade in captions for all figures in this gallery instead of the default slide-up behavior
- Many gallery styles for captions and hover effects exist; view the [hugo-easy-gallery GitHub](https://github.com/liwenyip/hugo-easy-gallery/) for all options
- Note that this theme will load the photoswipe gallery theme and scripts by default, no need to load photoswipe on your individual pages