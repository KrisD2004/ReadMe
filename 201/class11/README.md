# Audio, Video, Images

<https://css-tricks.com/snippets/css/complete-guide-grid/>

<https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content>

<https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images>

# CSS Grid

* CSS grid layout is a 2 dimensional grid-based layout system that compared to any web layout system of the past, completely changes the way we design user interfaces.
* CSS always been used to layout web pages but it never done a very good job of it.

## CSS Grid Animation

There are 5 different animation grid properties:

* Grid-gap, Grid-row-gap, grid-column-gap as length, percentage, or calc

* Grid-template-columns, grid-template-rows as a simple list of length, percentage, or calc, provided the only differences are the values of the length, percentage, or calc components in the list.

## CSS Grid terminology

* Grid container is the element on which display: grid is applied. It’s the direct parent of all the grid items.

* Grid line the dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column.

* Grid Track is the space between two adjacent grid lines. You can think of them as the columns or rows of the grid.

* Grid Area the total space surrounded by four grid lines. A grid area may be composed of any number of grid cells.

* Grid item the children of the grid container.

* Grid Cell the space between two adjacent row and two adjacent column grid lines. It’s a single “unit” of the grid.

# Video and audio content

* The video element allows you to embed a video very easily. 
Ex. <video src="rabbit320.webm" controls></video>

* Src In the same way as for the <img> element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.
* controls - the useres must be able control video and audio playback (it's especially critical for people who have epilepsy)!

## Questions 

1. The first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and Silverlight. 
2. In a similar manner to the <img> element, we include a path to the media we want to display inside the src attribute; we can include other attributes to specify information such as video width and height, whether we want it to autoplay and loop, whether we want to show the browser's default video controls, etc.
3. Fallback PTFs on the earlier-level release can allow it to tolerate changes that are made by the later-level release.In general, always plan to have a backout path when you install new software. Identify and install any service that is required to support backout.
4. CSS Grid Layout, is a two-dimensional grid-based layout system with rows and columns, making it easier to design web pages without having to use floats and positioning. Like tables, grid layout allow us to align elements into columns and rows
5. The CSS Flexbox offers a one-dimensional layout. It is helpful in allocating and aligning the space among items in a container (made of grids). It works with all kinds of display devices and screen sizes.