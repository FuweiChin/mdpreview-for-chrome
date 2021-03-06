# MDPreview
MDPreview is browser extension to preview Markdown files locally or on the web. It is forked from [GitHub Flavored Markdown](https://chrome.google.com/webstore/detail/github-flavored-markdown/faelggnmhofdamhdegcdhhemfokkfngk).

## Features
Compared to GitHub Flavored Markdown v0.0.6, MDPreview for Chrome 0.1 made the following changes:  
+ Added a Windows registry file md.reg to tell what the MIME type of `.md` file is.
+ Dropped type support for `.mdown` `.markdown`, added type support for `text/vnd.daringfireball.markdown`
+ Don't watch opened local file by default.  
  p.s. Users can set whether or not to watch opened local file in future release.
+ Support physical A4 21cm-width to preview content.  
  p.s. you need to customize relative DPI ratio according to your monitor in page.css. in my case it's `1.4709583133562356`, a.k.a. `Math.sqrt(1920*1920+1080*1080)/15.6/96`.

## Usage

### Windows
1. To preview markdown files locally, you need to nerge md.reg to registry.

### Chrome
1. Open Chrome, navigate to [chrome://extensions/](chrome://extensions/), enable developer mode and drop this folder into the Chrome Extensions page.
2. Open a `.md` file with Chrome locally, or visit any web `.md` resource with one of MIME types `text/plain` `text/markdown` `text/x-markdown` `text/vnd.daringfireball.markdown`.

### Firefox
1. Open Firefox, navigate to [about:debugging](about:debugging), click "Load temporary add-ons" and select manifest.json.
2. Open a `.md` file with Firefox locally, or visit any web `.md` resource with one of MIME types `text/plain` `text/markdown` `text/x-markdown` `text/vnd.daringfireball.markdown`.
