wp2octopress
============

Unimpressive Node.js application to generate Octopress posts from WordPress files.

Motivation
----------
I hated for all my old blog entries to disappear quietly.  And I really wanted to the backup
files off my hard drive so I can sleep at night.  So I created this repo so I don't lose the
knowledge I picked up through the exercise of creating this script.

Caution
-------
You would probably be better served by using something like [exitwp](https://github.com/thomasf/exitwp)
or using instructions like [these](http://vitobotta.com/how-to-migrate-from-wordpress-to-jekyll/).
Alas, I did not see these options before I dug in.

That said, please steal, mutilate, improve or do whatever you want with this script.

Method
------
My script assumes WordPress data has been exported into comma-separated variable (CSV) files.
I had an old backup of my [epmills.com](http://epmills.com) blog that I'd exported from my service
provider in the form of SQL files.  I imported them into MySQL and exported them using
[MySQL Workbench](http://www.mysql.com/products/workbench/).  This script reads the posts, terms and
taxonomies to gather enough information to generate a Markdown file with frontmatter for each post.

Acknowledgments
---------------
* [Node.js](http://nodejs.org)
* [Underscore](http://underscorejs.org/)
* [ya-csv](https://github.com/koles/ya-csv/)
* [Wrench](https://github.com/ryanmcgrath/wrench-js)
* [Async](https://github.com/caolan/async/)
* [to-markdown](https://github.com/domchristie/to-markdown)
* [node-slugs](https://github.com/Aaronontheweb/node-slugs)
