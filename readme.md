## Structure

```
// replace this with `tree` later
package.json
readme.md
license
build/
bin/
  - newPost
gulpfile.js/
  general
    merge-stream
    gulp-if
    lazypipe
    minification
    gulp-rev in prod
    source maps in dev
    gulp-load-plugins
    gulp-filter
    gulp-git
    gulp-rename
    browser-sync for dev
    fail hard in prod tasks; plumber dev
    gulp-useref? / gulp-processhtml? / gulp-preprocess?
    gulp-replace?
  - watch
  - clean
      del
  - build
      gulp-filesize
      gulp-size
      gulp-bump
      psi
  - deploy
      gulp-gh-pages
  - static (cname/robots/humans)
  - serve (local prod)
      gulp-connect?
      express?
  - sitemap
      gulp-sitemap?
  - feed
      node-rss?
  - favicon
      https://github.com/audreyr/favicon-cheat-sheet
  - images
      gulp-responsive?
      retina?
      gulp-imagemin
  - pages
      gulp-jade
  - posts
      frontmatter?
      speakingurl?
      markdown?
      tag page?
      blog page?
      minimize
      pagination / infinite scrolling?
      permalinks / slugs
      reading time?
      jade
  - scripts
      - something for console.log not showing in prod?
      browserify
      babel
      uglifyjs2
      velocity
      scrollmonitor
      headroom
      responsive-nav
      domready
      picturefill
      fastclick
      modernizr?
  - styles
      gulp-csso?
      gulp-cssimport
      gulp-cssnext
      mrmrs/colors
      https://github.com/sotayamashita/awesome-css#naming-conventions--methodologies
      corpuscss
      sanitize.css
      gulp-shorthand?
      clean-css
      myth?
      uncss?
      postcss?
      autoprefixer?
      jeet?
      grid?
source/
  - extras
    - CNAME       // for github url
    - robots.txt  // for search engines
    - humans.txt  // for nerds
    - sitemap.xml // for search engines
    - feed.xml    // for feed readers
    - favicon.ico // generate all favicons
  - images        // minify and rev
  - markup        // jade/md -> html
    - pages       // jade pages
    - posts       // md posts with frontmatter
    - templates   // jade templates used by pages + posts
  - scripts       // es6 + browserify -> js
    - blocking    // load in <header>
    - main        // load at end of <body>
  - styles        // stylus? -> css
```

good gulp examples:
- roots/sage
- vigetlabs/gulp-starter
- google/web-starter-kit
- cferdinandi/kraken
