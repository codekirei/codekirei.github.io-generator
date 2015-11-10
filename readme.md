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
    lazypipe
    minification
    gulp-rev in prod
    source maps in dev
    gulp-git
    gulp-data?
    browser-sync for dev
    fail hard in prod tasks; plumber dev
    gulp-useref? / gulp-processhtml? / gulp-preprocess?
    gulp-replace?
  - watch
  - clean
      del
  - build
      gulp-filesize
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
      ???
  - images
      gulp-responsive?
      retina?
      gulp-imagemin
  - pages
      gulp-jade
  - posts
      frontmatter?
      markdown?
      tag page?
      blog page?
      pagination / infinite scrolling?
      permalinks / slugs
      reading time?
      jade
  - scripts
      - something for console.log not showing in prod?
      browserify
      babel
      uglify
      modernizr?
  - styles
      gulp-csso?
      gulp-cssnext
      mrmrs/colors
      gulp-shorthand?
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
  - images        // favicon.ico -> favicons; images minified
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
