<div class="wrapper">
      <header>
        <h1>Danologia PWr</h1>
        <h3>Projekty</h3>
        
        {% if site.logo %}
          <img src="{{site.logo | relative_url}}" alt="Logo" />
        {% endif %}

        <p>{{ site.description | default: site.github.project_tagline }}</p>
        {{ content }}
<!--         {% if site.github.is_project_page %}
        <p class="view"><a href="{{ site.github.repository_url }}">View the Project on GitHub <small>{{ site.github.repository_nwo }}</small></a></p>
        {% endif %}
        
		### Witaj! 

		Po prawej znajdziesz listę projektów realizowanych przez studentów Danologii na studiach magisterskich na Politechnice Wrocławskiej. O kilku z nich można będzie usłyszeć podczas [Data Science Day](https://datascienceday.pl/) już 8 grudnia 2018 roku.

		
        {% if site.github.is_user_page %}
        <p class="view"><a href="{{ site.github.owner_url }}">View My GitHub Profile</a></p>
        {% endif %} -->

        {% if site.show_downloads %}
        <ul class="downloads">
          <li><a href="{{ site.github.zip_url }}">Download <strong>ZIP File</strong></a></li>
          <li><a href="{{ site.github.tar_url }}">Download <strong>TAR Ball</strong></a></li>
          <li><a href="{{ site.github.repository_url }}">View On <strong>GitHub</strong></a></li>
        </ul>
        {% endif %}
      </header>
      <section>
       {% include projectlist.html %}

      </section>
	  <footer>
<!--         {% if site.github.is_project_page %}
        <p>This project is maintained by <a href="{{ site.github.owner_url }}">{{ site.github.owner_name }}</a></p>
        {% endif %} -->
        <p><small>Hosted on GitHub Pages &mdash; Theme by <a href="https://github.com/orderedlist">orderedlist</a></small></p>
      </footer>
    </div>