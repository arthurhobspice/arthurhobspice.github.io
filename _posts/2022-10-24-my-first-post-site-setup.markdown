---
layout: post
title:  "My first post: site setup"
date:   2022-10-24 21:45:00 +0200
categories: it howtos
---
In the last few days I took some time to set up my GitHub Pages site. I dediced to use the <b>Jekyll</b> static
website generator as recommended by the GitHub Pages docs.

It's pretty straightforward, you can just follow the [GitHub Pages site creation with Jekyll howto][jekyll-gh-howto].

Install Jekyll as described in the [Jekyll docs][jekyll-docs].

Then create a GitHub repository for your site. In my case: `arthurhobspice.github.io`.

In a local folder, run `git init`, then `jekyll new --skip-bundle`. Edit the Gemfile as described in the howto,
so that the github-pages gem is activated. Save and close and run `bundle install`. Then you can view and test
your pages locally: run the "server" with `bundle exec jekyll serve` and open the URL [localhost:4000](http://localhost:4000) in your browser.
Changes to the files will automatically be applied (except for `_config.yml`, changes here require a restart of the server).
The locally generated content is in the `_site` subfolder (excluded by `.gitignore`).

Edit `_config.yml` to personalize the index page (header and footer). For example, I added an `author` definition and the
`linkedin_username`.

The site is created with the default "Minima" theme. I wasn't successful setting
another theme ("Cayman") so far, the local preview doesn't show the theme - left for later investigation.

After creation of a new document e.g. `unixtraining.markdown` with `layout:`, `title:` and `permalink:` definitions, the
header of the main (index) page gets a link to the new page automatically.

Finally, commit and push your site files to the GitHub repository. A few seconds later a GitHub Actions
workflow will publish your page.

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
[jekyll-gh-howto]: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll
