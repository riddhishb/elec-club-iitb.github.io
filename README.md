# Website of Electronics Club, IIT Bombay

## How to contribute
Create a fork from the source and then clone your local repo

<pre><span class="c"># clone your fork</span>
git clone https://github.com/username/elec-club-iitb.github.io

<span class="c"># add a tracking branch which can always have the last version of elec-club-iitb.github.io</span>
git remote add ec https://github.com/elec-club-iitb/elec-club-iitb.github.io
git fetch ec
git branch ec-master --track ec/master
git checkout ec-master
<span class="c"># you will only need to write the following command in to have the latest elec-club-iitb.github.io version</span>
git pull

<span class="c"># create a branch from the last dev version of the tracking branch above</span>
<span class="c"># let’s call this branch new_blog</span>
git branch new_blog
git checkout new_blog
<span class="c"># add and commit and push your changes at your default remote which is usually</span>
<span class="c"># called origin</span>
git add …
git commit …
git push origin new_blog

<span class="c"># make sure your branch is udpated with the latest changes in ec/master</span>
git checkout ec-master
git pull
git checkout new_blog
git merge ec-master

<span class="c"># If you see any conflicts you can resolve them using a standard and easy way.</span>
<span class="c"># Look for >>>> remove what is unnecessary and commit and push your changes</span>
git commit -am <span class="s2">"Resolved conflict"</span>
git push origin new_blog
</pre>

After you have finished pushing all your changes you are ready to make a pull request from github. You just need to press the green button from your github repo and write a title and a small description of what you are sharing with us.

After the pull request has arrived, the developers will review it and give you comments, and eventually merge it.



## How to write a blog post

Blog posts live in the `_posts` folder. They have specific filename format:

    yyyy-mm-dd-title.<ext>

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
