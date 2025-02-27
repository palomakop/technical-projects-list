# Technical Projects

*A list of my technical projects, and the tools used to create them*

## Personal Website

<img src="images/personal-website.jpg" alt="" width="250">

My homepage on the web, a space to display art projects and blog posts.

[Code Repository](https://github.com/palomakop/palomakop.tv-11ty/tree/main) | [Website Link](https://palomakop.tv)

**Tools used:**
- [Eleventy](https://11ty.dev) static site generator, which is built on [Node.js](https://nodejs.org/en)
- Automatic build & deploy via [Netlify](https://www.netlify.com/) triggered by each new commit to the Github repo

**Features:**
- Custom build configs written in JavaScript for shortcodes and other build-time goodies ([code](https://github.com/palomakop/palomakop.tv-11ty/blob/main/.eleventy.js))
- Custom video embeds via the [Vimeo Developer API](https://developer.vimeo.com/api/guides/start) allow me to get thumbnail images and provide a JavaScript-free fallback via the html5 `video` tag
- A custom music player written in JavaScript for embedding music albums ([demo](https://palomakop.tv/work/sleepwalks-tapes/), [code](https://github.com/palomakop/palomakop.tv-11ty/blob/main/src/js/musicplayer.js))
- A custom lightbox viewer in JavaScript for image galleries based on [Simple Lightbox](https://github.com/dbrekalo/simpleLightbox) ([demo - scroll down and click any image to open lightbox](https://palomakop.tv/work/synthetic-forest/))
- Custom templates written in [Liquid](https://shopify.github.io/liquid/)
- Font subsetting with [Python FontTools](https://github.com/fonttools/fonttools) for improved site load performance
- All site code was written from scratch (no starter templates were used)
