# The blog

# How to write a new article
1. Write the article
2. Create a new file in the `/_post` directory that follows the convention `YYYY-MM-DD-name-of-post.markdown`
3. The file consists of two part devided by `---`

    ```
    ---
    layout: post
    title:  "Title of your post"
    date:   2017-01-22 18:48:44 +0100
    author: your_name
    visible: 1
    categories: devided by space
    ---
    Here put your article in markdown
    ```

Don't forget to change the title, date, author and categories

5. Put your article into that file and style it properly
5. Test how your article will really look like.
6. Create commit and push to the master

# How to style the article
Articles are written in a markdown format.To have some inspiration how to use markdown,
see demo article in `inspiration_blog/2017-01-22-inspiration-blog.markdown` and
to see it on blog visit [this](http://abrt.github.io/the/inspiration/2017/01/22/inspiration-blog/)
page.

#Testing
When writing code it is normal to make errors. And since creating a new blog is
*"writing code"* you can make some as well. Therefore before pushing yours article
you should check three thinks:

1. Article does not include grammatical and typing errors
2. Article will be displayed
  * ...as a newest article
  * ...with correct title and date
3. Article is styled correctly

Testing of second two can be tricky, but thankfully there is a easy way of doing so.
First, you will need to install some Ruby gems. Please run:

    # dnf install rubygem-jekyll ruby-devel
    $ bundle install

Then you should be ready to run:

    $ bundle exec jekyll serve

This will locally deploy the whole website. Click a link provided by this command
(probably will be [http://localhost:4000](http://localhost:4000))

Now you can see the front page. Make sure your article is on the top, click it and
check it.

When you make change, there is no need to restart the local server - just let
it run and when file is edited, it will be automatically uploaded. You need to only
refresh the site in your browser.

## Credits
[Original theme](https://startbootstrap.com/template-overviews/clean-blog/) - modified a bit
