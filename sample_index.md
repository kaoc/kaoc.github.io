---
layout: page
title: Kerala Association of Colorado
subtitle: Fresh ideas with traditional values.
bigimg:
  - "/img/big-imgs/bigimg1.jpg" : ""
  - "/img/big-imgs/bigimg2.jpg" : ""
  - "/img/big-imgs/bigimg3.jpg" : ""
  - "/img/big-imgs/bigimg4.jpg" : ""

---
<h3> trial 4 </h3>
<table align="left" style="border:0">
	<col width="300">
	<col width="800">
	<col width="250">
	<tr style="border:0"><td style="border:0;background:light blue"><strong><font size="2px">upcoming events</font></strong></td><td style="border:0;background:transparent"></td><td style="border:0;background:transparent"></td></tr>
	<tr style="border:0"><td style="border:0;background:transparent">
<div class="row">
  <div class="col-md-8">
  	<!-- No upcoming events at present, please check back later! -->
  	<div class="posts-list">
  		{% for post in site.tags.upcoming-event reversed %}
			<article class="post-preview">
				{% if post.redirect_url %}
				<a href=" {{ post.redirect_url }}">
				{% else %}	
				<a href="{{ post.url | prepend: site.baseurl }}">
				{% endif %}
					<font size="4px">
						<strong>Event : {{ post.title }}</strong> </font><br/>				
				</a>
				<font size="2px">
					<strong>When : </strong> {{ post.date | date: "%B %-d, %Y" }} <br/>
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
			</article>
				<br/><br/>
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

</td><td style="border:0;background:transparent">
<font align="center">

Kerala Association of Colorado (<strong>KAOC</strong>) is a community driven cultural organization for Malayalees (‘Malayalam’ speaking people or the people from the South Indian state of Kerala) in Colorado, serving for more than 35 years. It acts as a bedrock for all types of arts and cultural activities for Keralites in Colorado.
<br/><br/>
		
<strong>KAOC</strong> is a registered non-profit organization exempt from taxes and certified per the federal regulations for non profit as a 501(c)(3) organization (Fed ID 84-1530554)

	
</font>
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
 
