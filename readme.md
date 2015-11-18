## Structure

```
// replace this with `tree` later
package.json
readme.md
license
build/
bin/
  - newPost
  - pagespeed (psi)
  - size
    - list sizes of major files in dist
  - deploy
    - bump version number
    - commit changes in dist sub-repo
    - push dist
  - css-parker -- analyze css complexity
  - css-stats -- analyze css with cssstats
  - css-guide -- generate style guide with postcss-style-guide
  - css-immutable -- use immutable-css to check for side effects
  - shots -- take screen shots with pageres
  - gremlins -- gremlins.js testing
gulpfile.js/
  general
    asset-builder
    merge-stream
    streamqueue
    lazypipe
    gulp-filter

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
    - img         // used in image tag
    - bg          // used in background tag
  - markup        // jade/md -> html
    - pages       // jade pages
    - posts       // md posts with frontmatter
    - templates   // jade templates used by pages + posts
  - scripts       // es6 + browserify -> js
    - main        // load at end of <body>
    - post        // post-specific scripts
  - styles        // stylus? -> css
```

good gulp examples:
- vigetlabs/gulp-starter
- roots/sage
- google/web-starter-kit
- cferdinandi/kraken
