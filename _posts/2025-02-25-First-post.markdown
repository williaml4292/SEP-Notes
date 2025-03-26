---
layout: post
title:  "My first post!"
date:   2025-02-24 14:09:28 -0500
categories: First post
permalink: /First-Post/
---
# Hello!
## This is my first post with Jekyll.

Post
{% assign var_1 = "6" %}
{% increment var_1 %}

{% increment var_1 %}
{{ var_1 }}

{% increment var_1 %}
{% increment var_1 %}

{% if var_1 == "3" %}
The variable is equals to 3.
{% else %}
No
{% endif %}

{% assign var_1 ="3" %}
{% if var_1 == "3" %}
{{ "The variable is equals to 3." | markdownify }}
{% else %}
No
{% endif %}
{{ Hi | downcase }}


{% highlight html linenos %}
 <p> Helllo </p>
  <p> Helllo </p>
   <p> Helllo </p>
{% endhighlight %}
