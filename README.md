# Default gallery setup for rgallery

This is the default gallery setup suggested for the [rgallery](https://github.com/dgrtwo/rgallery) package. It is a variation on the [Skinny Bones Jekyll Theme](http://mmistakes.github.io/skinny-bones-jekyll/) by [Michael Rose](https://mademistakes.com/).

To set up your page, you'll need [jekyll](http://jekyllrb.com/) and [rgallery](https://github.com/dgrtwo/rgallery) installed. Simply:

1. Clone the repository and enter the directory:

    git clone https://github.com/dgrtwo/rgallery-default.git my-gallery
    cd my-gallery

2. Start a Jekyll server:

    jekyll serve --watch

3. Visit your local gallery at [http://127.0.0.1:4000/](http://127.0.0.1:4000/).

4. To create additional snippets, add `.Rmd` files to the `_R` directory. Make sure you include `layout: snippet` in the YAML header.

5. To build (or re-build) your new snippets, go into R and run:

    rgallery::build_gallery()

That's it!
