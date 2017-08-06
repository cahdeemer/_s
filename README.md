[![Build Status](https://travis-ci.org/Automattic/_s.svg?branch=master)](https://travis-ci.org/Automattic/_s)

WordPress Basic Project, based on _s
===

Hi. I'm a WordPress basic project, base on `_s`, or `underscores`.  This project includes most of what is in `_s`, with some changes.

* includes Grunt
* includes Twitter Bootstrap CSS and JS files, already enqueued
* a simplified Sass structure

Getting Started, Part 1
---------------

Set up starts with the instructions for manual setup for `_s`.

The first thing you want to do is copy the `_s` directory and change the name to something else (like, say, `megatherium-is-awesome`), and then you'll need to do a five-step find and replace on the name in all the templates.

1. Search for `'_s'` (inside single quotations) to capture the text domain.
2. Search for `_s_` to capture all the function names.
3. Search for `Text Domain: _s` in style.css.
4. Search for <code>&nbsp;_s</code> (with a space before it) to capture DocBlocks.
5. Search for `_s-` to capture prefixed handles.

OR

* Search for: `'_s'` and replace with: `'megatherium-is-awesome'`
* Search for: `_s_` and replace with: `megatherium_is_awesome_`
* Search for: `Text Domain: _s` and replace with: `Text Domain: megatherium-is-awesome` in style.css.
* Search for: <code>&nbsp;_s</code> and replace with: <code>&nbsp;Megatherium_is_Awesome</code>
* Search for: `_s-` and replace with: `megatherium-is-awesome-`

Then, update the stylesheet header in `style.css` and the links in `footer.php` with your own information. Next, update or delete this readme.

Getting Started, Part 2
------------------

From terminal, run `npm install` to get all the dependencies.

Grunt Commands

`grunt`

Runs the basic watch command, which processes Sass and waits for changes.

`grunt startServer`

Runs a server on `localhost:4000` and watches for changes.

`grunt production`

Compiles Sass, removes console.log().
