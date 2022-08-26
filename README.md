# Setup

Open an account in [p5.js](https://editor.p5js.org/).

p5.js is a pretty handy editor for trying out ideas in sketches and, while simple to get started with, it provides a base for [some pretty impressive things](https://showcase.p5js.org/#/2021-All/The-ASL-Machine/) with the help of some other libraries.

You can save individual sketches in it, and for this project you should paste the starting code below.

# Introduction

[Fractals](https://en.wikipedia.org/wiki/Fractal_curve) are, loosely speaking, geometrical structures that can be divided in or gruped by parts, where each level has the same characteristics as those above or below, and [they occur naturally](https://webecoist.momtastic.com/2008/09/07/17-amazing-examples-of-fractals-in-nature/).

For example, the following fractal could be described as follows:

*Take the line segment, divide it in 3 subsegments, and break and pull the central subsegment from its middle point so that 2 lines result from it.*

![](https://georgemdallas.files.wordpress.com/2014/05/fractal4.jpg)

The interesting part is that these instructions can be applied to any (sub)segment in the figure, backwards and forwards: either subdividing to infinity, getting smaller and smaller "bumps" with each iteration, or undoing the process until the original line emerges.

# Challenge

We'll be dealing with the [Sierpiński triangle](https://en.wikipedia.org/wiki/Sierpi%C5%84ski_triangle).

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Sierpinski-Trigon-7.svg/1024px-Sierpinski-Trigon-7.svg.png)

Your job is to notice the fractal pattern in it and recreate it in p5.js.

We'll be keeping the details vague since it's a simple pattern and [p5.js has a pretty good documentation](https://p5js.org/reference/). Here's your starting code:

```
const canvasSize = 800;

// Called once
function setup() {
  createCanvas(canvasSize, canvasSize);

  angleMode(DEGREES);
}

// Called each frame
function draw() {
  background(220);
}
```

## Couldn't be that easy

* Can you animate it?
  * Leave each iteration on screen for a second, then move on to the next.
  * If you reach the maximum number of iterations (you did define a subdivision limit, didn't you?) then work your way backwards through them.
  * ⭐ Pretty ⭐ award.

* Can you make triangles selectable?
  * Click on a triangle. Fill it with a different color.
  * You might find [the area calculation approach](https://www.geeksforgeeks.org/check-whether-a-given-point-lies-inside-a-triangle-or-not/) useful for this.
  * ⭐ Is this UAT? ⭐ award.
