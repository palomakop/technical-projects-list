# Technical Projects

*A list of my technical projects, and the tools used to create them*

## Personal Website

<img src="images/personal-website.jpg" alt="" width="250">

My homepage on the web, a space to display art projects and blog posts.

[Code Repository](https://github.com/palomakop/palomakop.tv-11ty) | [Website Link](https://palomakop.tv)

**Tools used:**
- [Eleventy](https://11ty.dev) static site generator, which is built on [Node.js](https://nodejs.org/en)
- Automatic build & deploy via [Netlify](https://www.netlify.com/) triggered by each new commit to the Github repo

**Highlights:**
- Custom build configs written in JavaScript for shortcodes and other build-time goodies ([code](https://github.com/palomakop/palomakop.tv-11ty/blob/main/.eleventy.js))
- Custom video embeds via the [Vimeo Developer API](https://developer.vimeo.com/api/guides/start) allow me to get thumbnail images and provide a JavaScript-free fallback via the html5 `video` tag
- A custom music player written in JavaScript for embedding music albums ([demo](https://palomakop.tv/work/sleepwalks-tapes/), [code](https://github.com/palomakop/palomakop.tv-11ty/blob/main/src/js/musicplayer.js))
- A custom lightbox viewer in JavaScript for image galleries based on [Simple Lightbox](https://github.com/dbrekalo/simpleLightbox) ([demo - scroll down and click any image to open lightbox](https://palomakop.tv/work/synthetic-forest/))
- Custom templates written in [Liquid](https://shopify.github.io/liquid/)
- Font subsetting with [Python FontTools](https://github.com/fonttools/fonttools) for improved site load performance
- All site code was written from scratch (no starter templates were used)

## Community Infrastructure Hosting

Set-up and administration of online services for community organizations, all currently running on Hetzner virtual private servers

### Scanlines.xyz

<img src="images/scanlines.jpg" alt="" width="250">

An online community for people interested in DIY analog video circuits and art.

[Website Link](https://scanlines.xyz)

**Tools used:**
- The web forum runs on [Discourse](https://www.discourse.org/), an open-source forum software with a Rails back-end and an Ember.js front-end
- We also administrate a [Peertube instance](https://joinpeertube.org/) to provide video hosting to the community

**Highlights:**
- I built a custom Discourse theme component for a collapsible embedded chat widget. This became a proof-of-concept for an official plugin by Communiteq, a managed Discourse hosting service
- I also built a custom Discourse theme component for adding an embedded livestream video to the forum during live online events. This was used in conjunction with the custom chat widget to provide a Twitch-like live event experience
- Previously, we also ran a streaming server that used [an RTMP module for Nginx](https://github.com/sergey-dryabzhinsky/nginx-rtmp-module) to serve an HLS livestream video; this has been deprecated as Peertube has built-in video streaming

### Polyphase Portal

<img src="images/polyphase.jpg" alt="" width="250">

A cooperatively-run virtual school for online classes and workshops.

[Website Link](https://polyphaseportal.xyz)

**Tools used:**
- The main website is a [Wordpress](https://www.discourse.org/) instance, with Woocommerce and Stripe integration for ticket sales
- We run a [BigBlueButton instance](https://joinpeertube.org/) instance for video calls (it's an open-source Zoom alternative that's tailored to online teaching)
- We also run a [Matrix chat server]() to provide a space for connection outside of class time
- Our SSO server runs on [Keycloak]()

## Personal Projects

### The Lab

<img src="images/lab.jpg" alt="" width="250">

A minimal, text-adventure themed website to showcase small web-based projects and experiments.

[Code Repository](https://github.com/palomakop/lab) | [Website Link](https://lab.palomakop.tv)

**Tools used:**
- The static website is built with [Eleventy](https://11ty.dev) and deployed via [Netlify](https://www.netlify.com/), similarly to my main personal website
- Embedded interactive sketches created with:
  - [GLSL (fragment shaders)](https://www.khronos.org/opengl/wiki/Fragment_Shader)
  - [p5.js](https://p5js.org)
  - [Three.js](https://threejs.org/)
- The Three.js sketch features a 3D model created in [Houdini](https://www.sidefx.com/products/houdini/)

**Highlights:**
- A dark/light mode toggle that initializes based on the device color scheme (system-wide dark/light mode), then saves the toggled state in local storage for future visits
