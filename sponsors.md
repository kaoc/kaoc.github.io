---
layout: page
title: Our Esteemed Sponsors
subtitle: A BIG Thanks to our sponsors!
bigimg:
  - "/img/big-imgs/bigimg1.jpg" : ""
  - "/img/big-imgs/bigimg2.jpg" : ""
  - "/img/big-imgs/bigimg3.jpg" : ""
  - "/img/big-imgs/bigimg4.jpg" : ""
---
Major events are the Indian Dance Festival, Onam & Christmas Celebrations. Onam & Christmas Celebrations will have over 500 guests; Indian Dance Festival will have over 1000 guests. 

>These events are not possible without the support of **our generous Sponsors below!**

To more about sponsorship options, contact Vinod Kozhummal at [president@colorkerala.org](mailto:president@colorkerala.org)

<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_s-xclick">
<input type="hidden" name="hosted_button_id" value="38E8MVS458QC6">
<table>
<tr><td><input type="hidden" name="on0" value="Sponsorship Options">Sponsorship Options</td></tr><tr><td><select name="os0">
	<option value="Sponsorship Option-1">Sponsorship Option-1 $250.00 USD</option>
	<option value="Sponsorship Option-2">Sponsorship Option-2 $350.00 USD</option>
	<option value="Sponsorship Option-3">Sponsorship Option-3 $500.00 USD</option>
	<option value="Sponsorship Option-4">Sponsorship Option-4 $1,000.00 USD</option>
</select> </td></tr>
</table>
<input type="hidden" name="currency_code" value="USD">
<input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_paynowCC_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
<img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
</form>
<br>
<div id="container">
	{% for image in site.static_files %}
		{% if image.path contains 'sponsors/2018' %}
			<img src="{{ site.baseurl }}{{ image.path }}" alt="image" height="425" width="275"/>
		{% endif %}
	{% endfor %}
</div>

