Hello there!

My name is Oliver Reichweger, im 18 yeas old and I'm from Upper Austria.


## My public repositories
 
{% for repository in site.github.public_repositories %}

  {% unless repository.fork %}

- **[{{ repository.name }}]({{ repository.html_url }})**  

  ⭐ {{ repository.stargazers_count }} | 🍴 {{ repository.forks_count }}  

  _{{ repository.description }}_

  {% endunless %}

{% endfor %}
 
