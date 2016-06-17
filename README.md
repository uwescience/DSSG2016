# The UW eScience DSSG blog website

To create a new post:

- Clone this repo. Note that it does not have a `master` branch. Instead,
  The blog will get automatically generated from the `gh-pages` branch, so
  all the content needs to be added to this branch.

- Posts need to be added as new markdown files in the `_posts`. File names
  need to be something like `2016-06-16-example-post.md`. Note that the
  details in the header need to be something like:

>    ---
>    layout: post
>    title:  "Example Post"
>    date:   2016-06-16
>    author: Ariel Rokem
>    ---

  with your name, the title you want for your post, and the date you are
  writing it.

- To generate the site, we are using the [Jekyll](https://jekyllrb.com/)
  static website generator. For more information about the markdown syntax
  that you can use to write posts, add links, images, etc. Refer to the
  example post that is already there, and to the
  [Jekyll documentation](https://jekyllrb.com/docs/home/)



## Copyright & License

The template used for this website is Kasper, released under the following
license:

Copyright (C) 2013 Ghost Foundation - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
