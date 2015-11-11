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
    run-sequence
    requiredir
    streamqueue
    lazypipe
    sourcemaps
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
    gulp-size
    gulp-replace?
    incremental builds
    - changed
    - newer
    - cached
    - remember
source/
  - extras
    - CNAME       // for github url
    - robots.txt  // for search engines
    - humans.txt  // for nerds
    - sitemap.xml // for search engines
    - feed.xml    // for feed readers
    - crossdomain.xml
    - browserconfig.xml
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
- vigetlabs/gulp-starter
- roots/sage
- google/web-starter-kit
- cferdinandi/kraken
