# MVC for the web

## For the impatient

Start with `program-0.html`. Read the code and the extensive comments explaining the concepts. Open the file in a browser and play with it. When you understand it, move on to `program-1.html`, then to `program-2.html`, `program-3.html`, etc.

**Note**: There are many more examples yet to write. The programs here are barely the beginning of what needs to be conveyed.

## For the less impatient

The programs in this repository grew out of my attempts to learn how to write programs with graphical interfaces. Professionally, I needed to produce web interfaces, so I chose that substrate, though I chose to learn from the much more mature world of desktop environments, particularly Cocoa and Gtk+. This repository contains of a series of programs distilling what I have learned. They all use the set of techniques that go under the name of Model-View-Controller, or MVC.

MVC is often taken to be a particular architecture or organization of code. This is a misconception. MVC is a set of constraints that strongly limit how fast the complexity of code grows with the complexity of the user interface it implements. Some of the constraints isolate all user interface elements from each other via an intermediate layer, so the complexity of each user interface element is independent of how many others there are. Others organize user interface elements so they are easy to compose and reuse.

The examples consist of single, self contained HTML files. All CSS and JavaScript is inline in the HTML. None of the examples use any external libraries, nor have I felt their lack. Of particular note, I make full use JavaScript's prototype based object system. Trying to impose a class system in JavaScript is foolish, since the prototype based system is both simpler and more flexible. If you need to learn how to use JavaScript's object system, I recommend [You Don't Know JS: `this` and Object Prototypes](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/README.md#you-dont-know-js-this--object-prototypes).

The code depends on conservative choices of technology. The JavaScript is all ECMAScript 5. The page layouts use the traditional box model. I do use the HTML5 doctype and elements, but don't impose very onerous burdens on it. Everything should work in most modern browsers.

## Contents

* Program 0 - Observables
* Program 1 - Views
* Program 2 - View trees
* Program 3 - Deeper view trees

Material still to be written:
* Program 4 - Push protocols in models
* Program 5 - Reusable views and controllers
* Program 6 - Composite views
* Program 7 - Releasing views

Further material I plan to cover:
* Small multiples, sorting and filtering
* Interacting with remote servers: lazily loading data, and asynchronously writing data
* Form validation
* Working with the browser URL
* Undo/redo
* Layout managers in SVG and Canvas

## License

All the programs in this repository are licensed under the MIT License. See the LICENSE file for details.

## Authors

* Fred Ross (`fred at madhadron dot com`)

## Resources

* [Responsive web design patterns](http://bradfrost.github.io/this-is-responsive/patterns.html)
* [You Don't Know JS: `this` and Object Prototypes](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/README.md#you-dont-know-js-this--object-prototypes)