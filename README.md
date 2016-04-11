Preface
=======

This is a fork of an excellent Pure.css framework created for the purpose of tinkering and historical reasons. It was neither created, nor co-created by Likalo.com. You may find the original description of the Pure, along with copiright notices and desclaimenrs below this *preface*.
If you are looking for the original Pure.css, please use the information and links at hte bottom of this page to navigate to their original git page.

Pure
====
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/yahoo/pure?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Pure](https://cloud.githubusercontent.com/assets/449779/5291099/1b554cca-7b03-11e4-9157-53a12d91b34a.png)][Pure]

A set of small, responsive CSS modules that you can use in every web project.
[http://purecss.io/][Pure]

[Pure]: http://purecss.io/

Features
--------

Pure is meant to be a starting point for every website or web app. We take care
of all the CSS work that every site needs, without making it look cookie-cutter:

* A responsive grid that can be customized to your needs.

* A solid base built on [Normalize.css][] to fix cross-browser compatibility
  issues.

* Consistently styled buttons that work with `<a>` and `<button>` elements.

* Styles for vertical and horizontal menus, including support for dropdown
  menus.

* Useful form alignments that look great on all screen sizes.

* Various common table styles.

* An extremely minimalist look that is super-easy to customize.

* Responsive by default, with a non-responsive option.

* Extremely small file size: **4.5KB minified + gzip**.


[Normalize.css]: http://necolas.github.io/normalize.css/

Build From Source
-----------------

Optionally, you can build Pure from its source on Github. To do this, you'll
need to have Node.js and npm installed. We use [Grunt][] to build Pure.

```shell
$ git clone git@github.com:likalo/pure.git
$ cd pure
$ npm install
$ grunt
```

### Build Files

Now, all Pure CSS files should be built into the `pure/build/` directory. All
files that are in this build directory are also available on the CDN. The naming
conventions of the files in the `build/` directory follow these rules:

* `[module]-core.css`: The minimal set of styles, usually structural, that
  provide the base on which the rest of the module's styles build.

* `[module]-nr.css`: Rollup of `[module]-core.css` + `[module].css` +
  `[module]-[feature].css` from the `src/[module]/` dir. This is the
  non-responsive version of a module.

* `[module].css`: Rollup of `[module]-nr.css` + `[module]-r.css` from the
  `build/` dir. This is the responsive version of a module.

* `*-min.css`: A minified file version of the files of the same name.

* `pure.css`: A rollup of all `[module].css` files in the `build/` dir. This is
  a responsive roll-up of everything, non-minified.

* `pure-min.css`: Minified version of `pure.css` that should be used in
  production.

* `pure-nr.css`: A Rollup of all modules without @media queries. This is a
  non-responsive roll-up of everything, non-minified.

* `pure-nr-min.css`: Minified version of `pure-nr.css` that should be used in
  production.

* `grids-responsive.css`: Unminified version of Pure's grid stylesheet which 
  includes @media queries.

* `grids-responsive-min.css`: Minified version of `grids-responsive.css` that
  should be used in production.

* `pure-theme.css`: A Rollup of all skin modules. This includes
  colors and sizing for the framework.

* `pure-theme-min.css`: Minified version of `pure-theme.css` that should be used in
  production.

[Grunt]: http://gruntjs.com/


Browser Support and Testing
---------------------------

Pure is tested and works in:

* IE 8+
* Latest Stable: Firefox, Chrome, Safari
* iOS 6-8
* Android 4.x


License
-------

This software is free to use under the Yahoo! Inc. BSD license.
See the [LICENSE file][] for license text and copyright information.


[LICENSE file]: https://github.com/yahoo/pure/blob/master/LICENSE.md
