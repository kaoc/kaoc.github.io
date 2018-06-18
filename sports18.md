---
layout : page_auth_test
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script type = "text/javascript">
$(document).ready(function(){
$("#sel_danc_scl").hide();
$("#participant_dd_enb").hide();
$("#chg_par_nm").hide();
$("#ntrl").hide();
$(hide).click(function() {
$("p").toggle(1000);
});
$(show).click(function(){
$("p").show(1000);
});
$("#pull").click(function(){
$("#reel").slideDown("slow");
});
$("#pull").dblclick(function(){
$("#reel").slideUp("slow");
});

//$("#dnc_sch_nm").html( function (i,origText){return "<select id=\"dnc_sch_nm_txt\"> <option value=\"school1\">school1</option><option value=\"school2\">school2</option></select>"});
var dnc_sch_vr = document.createElement("dnc_sch_nm_txt");
dnc_sch_vr.innerHTML="<select id=\"dnc_sch_nm_txt\"> <option value=\"sch1\">sch1</option> <option value=\"sch2\">sch2</option> <option value=\"sch3\">sch3</option> </select>";
$("#dnc_sch_nm").append(dnc_sch_vr);

function enable_participant(){
$("#participant_dd_enb").show("slow");


var ppt_nm_vr = document.createElement("ppt_nm_txt");
if ($("#hid_dnc_sch_nm").val() == "sch1")
{
ppt_nm_vr.innerHTML="<select id=\"par_nm_txt_sel\"><option value=\"ps1\">ps1</option><option value=\"ps2\">ps2</option><option value=\"ps3\">ps3</option><option value=\"ps4\">ps4</option></select>";
}
else if ($("#hid_dnc_sch_nm").val() == "sch2")
{
ppt_nm_vr.innerHTML="<select id=\"par_nm_txt_sel\"><option value=\"ps21\">ps21</option><option value=\"ps22\">ps22</option><option value=\"ps23\">ps23</option><option value=\"ps24\">ps24</option></select>";
}
else if ($("#hid_dnc_sch_nm").val() == "sch3")
{
ppt_nm_vr.innerHTML="<select id=\"par_nm_txt_sel\"><option value=\"ps31\">ps31</option><option value=\"ps32\">ps32</option><option value=\"ps33\">ps33</option><option value=\"ps34\">ps34</option></select>";
}
$("#par_nm_txt").html("");
$("#par_nm_txt").append(ppt_nm_vr)
};

$("#dnc_sch_nm").change(function(){
//alert("change occurred"+$("#dnc_sch_nm_txt").val());
$("#hid_dnc_sch_nm").val($("#dnc_sch_nm_txt").val());
$("#dnc_sch_nm_txt").hide();
$("#dnc_sch_summ").html("<strong>you selected "+$("#hid_dnc_sch_nm").val()+"</strong>");
$("#sel_danc_scl").show("slow");
enable_participant();
$("#par_nm_txt").show();
$("#ntrl").show("slow");
});

$("#par_nm_txt").change(function(){
$("#hid_participant_nm").val($("#par_nm_txt_sel").val());
$("#par_nm_txt").hide();
$("#sel_par_nm").html("<strong>pp "+$("#hid_participant_nm").val()+"</strong>");
$("#sel_par_nm").show();
$("#chg_par_nm").show("slow");

});


$("#sel_danc_scl").click(function(){
$("#dnc_sch_summ").html("");
$("#dnc_sch_nm_txt").show();
$("#participant_dd_enb").hide();
$("#par_nm_txt_sel").hide();
$("#chg_par_nm").hide();
$("#sel_par_nm").hide();
$("#ntrl").hide("slow");
});

$("#chg_par_nm").click(function(){
$("#sel_par_nm").html("");
$("#par_nm_txt").show();

});


});
</script>

<script type="text/javascript" id="signup">
$(document).ready(function(){
var xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = function(){
if (this.readyState == 4 && this.state == 200){
	myFunction(this);
}
};
xhttp.open("GET","test.xml",true);
xhttp.send();

function myFunction(xml){
	var xmlDoc = xml.responseXML;
	var x = xmlDoc.getElementsByTagName("schoolnm")[0].childNodes[0];
	x.append(" school");
	document.getElementById("test").innerHTML = x.data;
}


});
</script>
<p> I am hidden </p>
<input type="button" id="hide" value="Hide Text"/>
<input type="button" id="show" value="Show Text" />
<table>
<tr><td style="background:green"> 
<div id="pull"> pulled the reel </div>
</td></tr>
<tr><td  style="background:red"> 
<div id="reel"> Data Is pulled </div>
</td></tr>
</table>
<input type="hidden" id="hid_dnc_sch_nm" />
<table>
<tr><td style="background:transparent">
<label> Please select the Dance School Name </label>
</td>
<td  style="background:transparent">
<div id="dnc_sch_nm"></div>
<div id="dnc_sch_summ"></div>
</td>
<td>
<div id="sel_danc_scl">change school</div>
</td>
</tr>
<input type="hidden" id="hid_participant_nm" />
<tr id="ntrl">
<div id="participant_dd_enb">
<td> 
<label> select participant name </label>
</td>
<td>
<div id="par_nm_txt"></div>
<div id="sel_par_nm"></div>
</td>
<td>
<div id="chg_par_nm">change participant</div>
</div>
</td>
</tr>
</table>

<table id="signup">
<tr><td>Sample value goes here<div id="test"></div></td></tr>
</table>
