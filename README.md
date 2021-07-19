# PANZOOM
Panzoom is a small library (~3.7kb gzipped) to add panning and zooming functionality to an element. Rather than using absolute positioning or setting width and height, Panzoom uses CSS transforms to take advantage of hardware/GPU acceleration in the browser, which means the element can be anything: an image, a video, an iframe, a canvas, text, WHATEVER.

# Visit to documentation page on github

https://github.com/timmywil/panzoom#readme

# Installing

Download PANZOOM Jquery plugin
https://github.com/timmywil/panzoom

or visit to jqueryscript.net
https://www.jqueryscript.net/blog/Best-Image-Zoom-jQuery-Plugins.html

With a script tag:
<script src="/js/panzoom.js"></script>

# Usage

const elem = document.getElementById('panzoom-element')
const panzoom = Panzoom(elem, {
  maxScale: 5
})
panzoom.pan(10, 10)
panzoom.zoom(2, { animate: true })

// Panning and pinch zooming are bound automatically (unless disablePan is true).
// There are several available methods for zooming
// that can be bound on button clicks or mousewheel.
button.addEventListener('click', panzoom.zoomIn)
elem.parentElement.addEventListener('wheel', panzoom.zoomWithWheel)

