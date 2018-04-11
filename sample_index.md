---
layout: page
title: Kerala Association of Colorado
subtitle: Fresh ideas with traditional values.
bigimg:
  - "/img/big-imgs/bigimg1.jpg" : ""
  - "/img/big-imgs/bigimg2.jpg" : ""
  - "/img/big-imgs/bigimg3.jpg" : ""
  - "/img/big-imgs/bigimg4.jpg" : ""
css: infinite-scrolling-photo-banner-test.css
---
<h1> trial 2 </h1>
<table>
	<tr><td>
<div class="row">
  <div class="col-md-8">
  	<!-- No upcoming events at present, please check back later! -->
  	<div class="posts-list">
  		{% for post in site.tags.upcoming-event reversed %}
			<article class="post-preview">
				<a href="{{ post.url | prepend: site.baseurl }}">
					<strong>{{ post.title }}</strong>
				</a>
				<p class="post-meta">
					Event will be held on {{ post.date | date: "%B %-d, %Y" }}
				</p>
			</article>
  		{% endfor %}
	</div>
  </div>
	
  <!-- <div class="col-md-2 col-md-offset-1">
  	Our online printing service partner!
  	<a href="https://smartpress.com">
  	   <img src="/img/sponsors/smartpress-logo-blue-horizontal-png.png" alt="Smartpress.com logo" height="40" width="240"/>
	</a>
  </div> -->
  
</div>
{% if paginator.total_pages > 1 %}
	<ul class="pager main-pager">
  	{% if paginator.previous_page %}
  	<li class="previous">
    	<a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  	</li>
  	{% endif %}
  	{% if paginator.next_page %}
  	<li class="next">
    	<a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  	</li>
  	{% endif %}
	</ul>
	{% endif %}
</td><td> About KAOC </td></tr>
<tr><td>
</td></tr>
</table>	
<div id="container">
    <div class="photobanner">
		{% for image in site.static_files %}
			{% if image.path contains 'sponsors/2018/02' %}
				<a href="{{ site.baseurl }}{{ image.path }}"><img class="first" src="{{ site.baseurl }}{{ image.path }}" alt="image" height="200" width="180"/></a>
			{% endif %}
		{% endfor %}
        <!-- REPEAT First few sponsors-->	
	    {% for image in site.static_files %}
			{% if image.path contains 'sponsors/2018/0' %}
				<a href="{{ site.baseurl }}{{ image.path }}"><img class="first" src="{{ site.baseurl }}{{ image.path }}" alt="image" height="200" width="180"/></a>
			{% endif %}
		{% endfor %}
    </div>
</div>

