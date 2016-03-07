# Website of Electronics Club, IIT Bombay

## How to write a blog post

Blog posts live in the `_posts` folder. They have specific filename format:

    yyyy-mm-dd-<title>.<ext>

`<title>` should be lowercase of the words of your title seperated by a '`-`' ( hyphen ). 

`<ext>` should be the file-format extension. You can write the blog post in HTML ('html' extension) or Markdown ('md' extension). Markdown is a simple and intuitive markup language (preferrable over HTML). [Here's](https://daringfireball.net/projects/markdown/basics) a good tutorial for it. If you do use HTML, keep it to simple tags like `<h1>`, `<p>`, `<img>` and such.

For eg.

    2016-03-07-first-post.md

Content of the file should include this Front Matter on top:

    ---
    layout: post
    comments: true

    title: First Post
    excerpt: Small description for main page
    author: Your Name
    category: [Electronics, Robotics]
    tags: [Raspberry Pi, Arduino]
    ---

        ...
        content
        ...

Change the `title`, `excerpt`, `author`, `category` and `tags` field appropriately. They will be used to generate title and description of your blog on the homepage, and will add it to corresponding category and tag-wise pages.

There is no need to add title or date in the content, they will be added automatically.

So just fork, add a post and send a PR, or just push it directly here if you have access!

## Theme
[Jekyll Experiment](https://github.com/tokkonopapa/jekyll-experiment)
