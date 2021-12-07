---
title: "Welcome to Jekyll!"
date: 2019-04-18T15:34:30-04:00
categories:
  - blog
tags:
  - Jekyll
  - update
toc: true
toc_sticky: true
mathjax: true
last_modified_at: 2021-12-07T15:34:30-04:00
---

Hello World 😀!

# Intro
You'll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

# Code snippets playground
Jekyll also offers powerful support for code snippets:

{% highlight ruby linenos %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```
# Math playground.
When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are:
\[x = {-b \pm \sqrt{b^2-4ac} \over 2a}\]

\[\begin{multline}
\shoveleft
\begin{aligned}
G_t&=R_{t+1}+\gamma R_{t+2}+\gamma^2 R_{t+3}+\gamma^3 R_{t+4}+...\newline
&=R_{t+1}+\gamma(R_{t+2}+\gamma R_{t+3}+\gamma^2 R_{t+4})+...\newline
&=R_{t+1}+\gamma G_{t+1}\newline
\end{aligned}
\end{multline}\]

# Toggle list test
<details>
  <summary>Click to expand!</summary>
  
  {% capture toggle-1 %}
  ## Code below
  Something to write about.

  ```javascript
    function logSometing(something) {
      console.log(`Logging: ${something}`);
    }
  ```
  {% endcapture %}

  <div class="notice">{{ toggle-1 | markdownify }}</div>
</details>

# Footnotes
Testing footnotes. [^1]

[^1]: <http://en.wikipedia.org/wiki/Syntax_highlighting>

# More info
Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
