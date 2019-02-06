---
layout: page
title: Kerala Association of Colorado
subtitle: Fresh ideas with traditional values.
bigimg:
  - "/img/big-imgs/col04.jpg" : ""
  - "/img/big-imgs/col08.jpg" : ""
  - "/img/big-imgs/ker05.jpg" : ""
  - "/img/big-imgs/ker07.jpg" : ""

---
<table align="left" style="border:0">
	<col width="400">
	<col width="800">
	<col width="250">
	<tr style="border:0;background:transparent"><td style="border:0;background:transparent">
<div class="row">
  <div class="col-md-8">
  	<!-- No upcoming events at present, please check back later! -->
  	<div class="posts-list">
		<table align="left" style="border:0">
		<col width="300">
		{% for post in site.tags.upcoming-event reversed %}
			<tr style="border:0;background:transparent"><td style="border:0;background:transparent">
			<article class="post-preview">
				{% if post.redirect_url %}
				<a href=" {{ post.redirect_url }}">
				{% else %}	
				<a href="{{ post.url | prepend: site.baseurl }}">
				{% endif %}
					<font size="3px">
						<strong>Event : {{ post.title }}</strong> </font><br/>				
				</a>
				<font size="2px">
				{% if post.between %}
					<strong>Between : </strong> {{post.between}} <br/>
				{% else %}
					{% if post.endon %}
						<strong>Last Date  : </strong> {{post.endon}} <br/>
					{% else %}
						<strong>When : </strong> {{ post.date | date: "%B %-d, %Y" }} <br/>
					{% endif %}
				{% endif %}	
				</font>	
				{% if post.time%}
					<font size="2px">
					<strong>Time : </strong>{{ post.time }}	<br/> 
					</font>	
				{% endif %}
				{% if post.location %}
					<font size="2px">
					<strong>Where : </strong> {{ post.location }} <br/>
					</font>	
				{% endif %} 
				{% if post.address %}					
					<table align= "left" style="border:0"><tr style="border:0;background:#cccccc"><td style="border:0">
					<font size="1px"> {{ post.address }} </font><br/>
						</td></tr></table>	
				{% endif %} 	
			
				{% if post.message %}
					<font size="2px">
						{% if post.redirect_url %}
							<a href=" {{ post.redirect_url }}">
						{% else %}	
							<a href="{{ post.url | prepend: site.baseurl }}">
						{% endif %}
								{{ post.message }} </a><br/>
					</font>	
				{% endif %}
				</article><br/><br/>
				</td></tr>
  		{% endfor %}
				</table>
	</div>
  </div>
	
  <!-- <div class="col-md-2 col-md-offset-1">
  	Our online printing service partner!
  	<a href="https://smartpress.com">
  	   <img src="/img/sponsors/smartpress-logo-blue-horizontal-png.png" alt="Smartpress.com logo" height="40" width="240"/>
	</a>
  </div> -->
  
</div>

</td><td style="border:0;background:transparent">
<table align="left" style="border:0">
<tr style="border:0;background:transparent"><td style="border:0;background:transparent">
<font align="center">
Kerala Association of Colorado (<strong>KAOC</strong>) is a community driven cultural organization for Malayalees (‘Malayalam’ speaking people or the people from the South Indian state of Kerala) in Colorado, serving for more than 35 years. It acts as a bedrock for all types of arts and cultural activities for Keralites in Colorado.
<br/>		
 <a href="https://www.colorkerala.org/about-kaoc-history/" > read more </a>
<br/> <br/> <br/>
	<a href="https://www.colorkerala.org/upcoming-events/"> click here to view all events and dates (including tentative) </a>
</font>

	</td></tr></table>
</td><td style="border:0;background:transparent">
	<div id="sponsors">
	    	<marquee behaviour="scroll" direction="up" height="600" scrollamount="3" style="height:600px;width:300px;" width="800px">
	{% for image in site.static_files %}	    	
		{% if image.path contains 'sponsors/2018/' %}
			<div> <a href="{{ site.baseurl }}{{ image.path }}"> <img src="{{ site.baseurl }}{{ image.path }}" style="height:600px;width:250px" align="center"/></a> </div><br/>
	    	{% endif %}
	{% endfor %}
	     </marquee> 
			</div>
	</td></tr>
	</table>
 
 
