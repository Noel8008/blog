# Welcome to Noel's Blog :3

Hello World My name is [Noel Singh](https://noel8008.github.io) and I am in the 12th grade at [Boys and Girls High-School](https://www.youtube.com/watch?v=ZmqgIHbeXnA) and I'm a current Full-Stack Development and Programming Student at the [Brooklyn Steam Center](https://brooklynsteamcenter.org). I'm **6'1**. This will be my blog about..

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
