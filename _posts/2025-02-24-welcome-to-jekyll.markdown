---
title:  "Jekyll Summary"
date:   2025-02-24 14:09:28 -0500
categories: jekyll-update
permalink: /welcome-to-jekyll/
---
{{ page.author }}

{% if author2 contains "Hello" %}
The statement is true
{% else %}
False
{% endif %}



This is a second one.
{% capture author2 %}
{{ page.author }}, a student from HSTAT.
{% endcapture %}
{{ author2 }}

{% assign hobbies = "reading and videogames." %}

{% capture introduction %}
Hello, my name is {{ author2 }} My hobbies are {{ hobbies }}
{% endcapture %}
{{ introduction }}


{% assign smoothie_flavors = "orange, strawberry, banana, computers" | split: ", " %}

{% for flavor in smoothie_flavors -%}

    {{ flavor }}{% unless forloop.last %} - {% endunless -%}

{% endfor %}

{% assign text = author2 %}

{% if author2 contains "page.author" %}
The statement is true
{% else %}
False
{% endif %}

{{ text }}


You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
