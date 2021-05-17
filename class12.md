# Charts
Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create

 1. **Setting up**
- The first thing we need to do is [download Chart.js.]()
Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in

 2. **Drawing a line chart**
- To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart.

- write a script that will retrieve the context of the canvas, so add this to the foot of your body element

 3. **Drawing a pie chart**

4. **Drawing a bar chart**

*The great things about Chart.js are that it’s simple to use and really very flexible. Plus, once you’vemastered the basics here, you’ll discover that there are tons of options*

## Basic usage of canvas
**The < canvas > element**
At first sight a < canvas > looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes.

**Fallback content**
The < canvas> element differs from an < img> tag in that, like for < video>, < audio>, or < picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

![canvas](https://www.webfx.com/blog/images/assets/images.sixrevisions.com/2010/10/03-01_html5_canvas_element_ld_img.png)

*The script includes a function called draw(), which is executed once the page finishes loading*

### Drawing shapes with canvas

 < canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths.

 **Applying styles and colors**

 **Colors**
Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

*fillStyle = color*

**Transparency**
In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

*globalAlpha = transparencyValue*

### Drawing text
The canvas rendering context provides two methods to render text:

*fillText(text, x, y [, maxWidth])*
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
*strokeText(text, x, y [, maxWidth])*
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.



