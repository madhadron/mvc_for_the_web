# MVC for the web

## For the impatient

Start with `program-0.html`. Read the code and the extensive comments explaining the concepts. Open the file in a browser and play with it. When you understand it, move on to `program-1.html`, then to `program-2.html`, `program-3.html`, etc.

**Note**: There are many more examples yet to write. The programs here are barely the beginning of what needs to be conveyed.

## Contents

* [Program 0 - Observables](program-0.html)
* [Program 1 - Views](program-1.html)
* [Program 2 - View trees](program-2.html)
* [Program 3 - Deeper view trees](program-3.html)
* [Program 4 - Push protocols in models](program-4.html)
* [Program 5 - Reusable views and controllers](program-5.html)
* [Program 6 - More reusable views and controllers](program-6.html)
* [Program 7 - Composite views](program-7.html)
* [Program 8 - Manipulating the URL](program-8.html)
* [Program 9 - Releasing views](program-9.html)
* [Program 10 - Small multiples - Lists](program-10.html)

## For the less impatient

The programs in this repository grew out of my attempts to learn how to write programs with graphical interfaces. Professionally, I needed to produce web interfaces, so I chose that substrate, though I chose to learn from the much more mature world of desktop environments, particularly Cocoa and Gtk+. This repository contains of a series of programs distilling what I have learned. They all use the set of techniques that go under the name of Model-View-Controller, or MVC.

MVC is often taken to be a particular architecture or organization of code. This is a misconception. MVC is a set of constraints that strongly limit how fast the complexity of code grows with the complexity of the user interface it implements. Some of the constraints isolate all user interface elements from each other via an intermediate layer, so the complexity of each user interface element is independent of how many others there are. Others organize user interface elements so they are easy to compose and reuse.

The examples consist of single, self contained HTML files. All CSS and JavaScript is inline in the HTML. None of the examples use any external libraries, nor have I felt their lack. Of particular note, I make full use JavaScript's prototype based object system. Trying to impose a class system in JavaScript is foolish, since the prototype based system is both simpler and more flexible. If you need to learn how to use JavaScript's object system, I recommend [You Don't Know JS: `this` and Object Prototypes](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/README.md#you-dont-know-js-this--object-prototypes).

The code depends on conservative choices of technology. The JavaScript is all ECMAScript 5, except for using ECMAScript 6's Set collection, which is fairly broadly supported. The page layouts use the traditional box model. I do use the HTML5 doctype and elements, but don't impose very onerous burdens on it. Everything should work in most modern browsers.

## Further work

Material still to be written:
* Sorting and filtering small multiples - Tables
* Tabs again as small multiples
* Loading and syncing to remote models
* Lazily loading data
* Composing models - Control states and actions
* Drag and drop
* Undo/redo
* Pluralization

Techniques that I want to revise:
* Make Observable a constructor function instead of trying to provide a prototype.
* Revise Controllers so they don't need an initialize method.
* Factor out rendering a sequence of subviews into a single function.
* Adding and removing classes from elements in a structured way.

Technologies that I wish were ready, but aren't broadly enough supported:
* HTML5 context menus
* Flexboxes
* Grid layout
* Internationalization API (ECMA 402)
* ECMAScript 6 modules

Code that would be worth pulling out for reuse:
* Observable
* Root views such as Body and TwoColumn
* UrlView
* Widgets such as Button, Label, and TextBox

## License

All the programs in this repository are licensed under the MIT License. See the LICENSE file for details.

## Authors

* Fred Ross (`fred at madhadron dot com`)

## Resources

* [Responsive web design patterns](http://bradfrost.github.io/this-is-responsive/patterns.html)
* [You Don't Know JS: `this` and Object Prototypes](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/README.md#you-dont-know-js-this--object-prototypes)
