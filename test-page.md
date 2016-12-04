---
layout: page
title: Kerala Association of Colorado
subtitle: Fresh ideas with traditional values.
bigimg:
  - "/img/big-imgs/bigimg1.jpg" : ""
  - "/img/big-imgs/bigimg2.jpg" : ""
  - "/img/big-imgs/bigimg3.jpg" : ""
  - "/img/big-imgs/bigimg4.jpg" : ""
css: /css/infinite-scrolling-photo-banner.css
---
<div class="row">
  <div class="col-md-8" class="posts-list">
  		{% for post in site.tags.upcoming-event %}
  		<article class="post-preview">
    		<a href="{{ post.url | prepend: site.baseurl }}">
	  	<h2 class="post-title">{{ post.title }}</h2>

	  	{% if post.subtitle %}
	  	<h3 class="post-subtitle">
	    	{{ post.subtitle }}
	  	</h3>
	  	{% endif %}
    		</a>

    		<p class="post-meta">
      			Event will be held on {{ post.date | date: "%B %-d, %Y" }}
    		</p>

    		<div class="post-entry">
      		{{ post.content | strip_html | xml_escape | truncatewords: 50 }}
	  		<a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
    		</div>

    		{% if post.tags.size > 0 %}
    		<div class="blog-tags">
      		Tags: 
      			{% if site.link-tags %}
      			{% for tag in post.tags %}
      			<a href="{{ site.baseurl }}/tag/{{ tag }}">{{ tag }}</a>
      		{% endfor %}
      		{% else %}
        		{{ post.tags | join: ", " }}
      		{% endif %}
    		</div>
    		{% endif %}

   		</article>
  		{% endfor %}
	</div>
  	<div class="col-md-4"><img src="/img/sponsors/promo1.jpg" alt="" height="170" width="240"/></div>
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
</div>
<div id="container">
    <!-- Each image is 350px by 233px -->
    <div class="photobanner">
    	<img class="first" src="/img/sponsors/sponsor1.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor2.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor3.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor4.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor5.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor6.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor7.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor8.jpg" alt="" height="155" width="224"/>
	<img src="/img/sponsors/sponsor9.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor10.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor11.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor12.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor13.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor14.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor15.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor16.jpg" alt="" height="155" width="224"/>
	<img src="/img/sponsors/sponsor17.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor18.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor19.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor20.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor21.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor22.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor23.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor24.jpg" alt="" height="155" width="224"/>
	<img src="/img/sponsors/sponsor25.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor26.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor27.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor28.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor29.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor30.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor31.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor32.jpg" alt="" height="155" width="224"/>
	<img src="/img/sponsors/sponsor33.jpg" alt="" height="155" width="224"/>
	<img src="/img/sponsors/sponsor34.jpg" alt="" height="155" width="224"/>
	<img src="/img/sponsors/sponsor35.jpg" alt="" height="155" width="224"/>
        <!-- REPEAT First 5 sponsors-->	
	<img src="/img/sponsors/sponsor1.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor2.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor3.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor4.jpg" alt="" height="155" width="224"/>
    	<img src="/img/sponsors/sponsor5.jpg" alt="" height="155" width="224"/>
    </div>
</div>
