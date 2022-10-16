# Class 11 Notes - Audio, Video, Images

[Back to Home](../README.md)

#### Bookmarks - [Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML) and [Embedding Techologies](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Other_embedding_technologies)

## [Video and Audio Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

1) Explain how the ability to use video and audio on the web has evolved since the early 2000s.

+ The first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and SilverLight
+ Both of these had security and accessibility issues, and are now obsolete, in favor of native HTML solutions `<video>` and `<audio>` elements and the availability of JavaScript APIs for controlling them

2) Describe the use of the `src` and `controls` attributes in the `<video>` element.

+ src - In the same way as for the `<img>` element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.
+ controls - You must either use the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.

3) Why is it important to have fallback content inside the `<video>` element?

+ this will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

4) Write a very short story where `<audio>` and `<video>` are characters.

+ Audio and video walk into a bar. The bartender says what's your source? Audio and video say which one do you mean, we have multiple. Always have a backup.

## [CSS - Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

1) How does Grid layout differ from Flex?

+ Flex box is great but it is one directional.
+ Grid is the very first CSS module created specifically to solve the layout problems we’ve all been hacking our way around for as long as we’ve been making websites.

2) Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

+ Grid container - The element on which display: grid is applied. It’s the direct parent of all the grid items. 
+ grid item - The children (i.e. direct descendants) of the grid container. Here the item elements are grid items
+ Grid line - The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.
+ also grid cell and grid track and grid area

## [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

1) Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

+ The general problem whereby you want to serve different cropped images in that way, for various layouts, is commonly known as the `art direction problem`.
+ the resolution switching problem.
+ Conversely, it is unnecessary to display a large image on a screen significantly smaller than the size it was meant for. Doing so can waste bandwidth; in particular, mobile users don't want to waste bandwidth by downloading a large image intended for desktop users

2) Define the following `<img>` attributes srcset and sizes. Write an example of how they are used.

+ srcset - defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma.
+ sizes - defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true

3) How is srcset more helpful for responsive images than CSS or JavaScript?

+  If you're supporting multiple display resolutions, but everyone sees your image at the same real-world size on the screen, you can allow the browser to choose an appropriate resolution image by using srcset with x-descriptors and without sizes — a somewhat easier syntax! 
+ When the browser starts to load a page, it starts to download (preload) any images before the main parser has started to load and interpret the page's CSS and JavaScript. That mechanism is useful in general for reducing page load times, but it is not helpful for responsive images — hence the need to implement solutions like srcset. For example, you couldn't load the <img> element, then detect the viewport width with JavaScript, and then dynamically change the source image to a smaller one if desired. By then, the original image would already have been loaded, and you would load the small image as well, which is even worse in responsive image terms
