# center.js
Center.js is jQuery library to make element center as compared to his outside element. It's also work in responsive.
<style>
pre{
	background-color: black;
    color: white;
    border-radius: 3px;
    padding: 0px 20px;
	line-height:1.3;
	word-wrap: break-word;
	margin: 10px 0px 20px;
}
pre code br{
	display:none;
}
p{
    display: inline-block;
	margin: 0px 0px 10px 0px;
    padding: 0px;
	font-size: 14px;
    font-weight: normal;
}
.header{
	text-align:center;
}
h2{
	font-size: 20px;
    padding: 0px;
    margin: 40px 0px 5px;
}
.center{
	width:100%;
	border:1px solid black;
	padding:100px 100px;
}
.center div{
	height:200px;
	width:70%;
	border:1px solid black;
}
.mvcenter{
	width:100%;
	border:1px solid black;
	height:500px;
}
.mvcenter div:nth-of-type(1){
	width:20%;
	height:25%;
	border:1px solid black;
}
.mvcenter div:nth-of-type(1) div{
	width:70%;
	height:50%;
}

.mvcenter div:nth-of-type(2){
	width:25%;
	height:30%;
	border:1px solid black;
}
.mvcenter div:nth-of-type(2) div{
	width:50%;
	height:70%;
}
.mvcenter div:nth-of-type(3){
	width:30%;
	height:30%;
	border:1px solid black;
}
.mvcenter div:nth-of-type(3) div{
	width:30%;
	height:30%;
}
.vcenter, .hcenter{
	width:100%;
	border:1px solid black;
	height:400px;
}
.vcenter div, .hcenter div{
	width:30%;
	height:30%;
	border:1px solid black;
}
</style>
<h2>1. data-center </h2>
<p>( Horizontally and vertically center with single element )</p>
<p>This for first we need to assign outside element to data-box. Then need to assign inside element to data-center. So here inside element set center as compared to his outside element.</p>
<pre>
  <code>
&lt;div class="center" data-center data-box&gt;<br />
	&lt;div data-center data-box&gt;&lt;p data-center&gt;data-center&lt;/p&gt;&lt;/div&gt;<br />
&lt;/div&gt;
  </code>
</pre>
<div class="center" data-box>

	<div data-center data-box><p data-center>data-center</p></div>
</div>

<h2>2. data-mvcenter <p>( Vertically center with multipal element )</p></h2>
<p>This for first we need to assign outside element to data-box. Then need to assign inside element to data-mvcenter. So here all inside element set vertically center as compared to his outside element.</p>
<pre>
  <code>
&lt;div class="mvcenter" data-box&gt;<br />

    &lt;div data-mvcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;<br />
    &lt;div data-mvcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;<br />
    &lt;div data-mvcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;<br />
&lt;/div&gt;
  </code>
</pre>
<div class="mvcenter" data-box>
	<div data-mvcenter data-box><p data-center>data-mvcenter</p></div>
    <div data-mvcenter data-box><p data-center>data-mvcenter</p></div>
    <div data-mvcenter data-box><p data-center>data-mvcenter</p></div>
</div>
<h2>3. data-mhcenter <p>( Horizontally center with multipal element )</p></h2>
<p>This for first we need to assign outside element to data-box. Then need to assign inside element to data-mhcenter. So here all inside element set horizontally center as compared to his outside element.</p>
<pre>
  <code>
&lt;div class="mvcenter" data-box&gt;<br />
    &lt;div data-mhcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;<br />
    &lt;div data-mhcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;<br />
    &lt;div data-mhcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;<br />
&lt;/div&gt;
  </code>
</pre>
<div class="mvcenter" data-box>
	<div data-mhcenter data-box><p data-center>data-mvcenter</p></div>
    <div data-mhcenter data-box><p data-center>data-mvcenter</p></div>
    <div data-mhcenter data-box><p data-center>data-mvcenter</p></div>
</div>

<h2>4. data-vcenter <p>( Vertically center with single element )</p></h2>
<p>This for first we need to assign outside element to data-box. Then need to assign inside element to data-vcenter. So here inside element set vertically center as compared to his outside element.</p>
<pre>
  <code>
&lt;div class="vcenter" data-box&gt;<br />
	&lt;div data-vcenter data-box&gt;&lt;p data-center&gt;data-vcenter&lt;/p&gt;&lt;/div&gt;<br />
&lt;/div&gt;
  </code>
</pre>
<div class="vcenter" data-box>
	<div data-vcenter data-box><p data-center>data-vcenter</p></div>
</div>
<h2>5. data-hcenter <p>( Horizontally center with single element )</p></h2>
<p>This for first we need to assign outside element to data-box. Then need to assign inside element to data-hcenter. So here inside element set horizontally center as compared to his outside element.</p>
<pre>
  <code>
&lt;div class="hcenter" data-box&gt;<br />
	&lt;div data-hcenter data-box&gt;&lt;p data-center&gt;data-hcenter&lt;/p&gt;&lt;/div&gt;<br />
&lt;/div&gt;
  </code>
</pre>
<div class="hcenter" data-box>
	<div data-hcenter data-box><p data-center>data-hcenter</p></div>
</div>
<h2>Use multiple data</h2>
<p>Here below example in show that one data-box inside onther data-box. So we can use multipal center.js element (data-center, data-vcenter, data-hcenter, data-mvcenter, data-mhcenter). But we can't use one data-box in child in multipal center.js element.</p>
<pre>
  <code>
&lt;div class="mvcenter" data-box&gt;<br />
    &lt;div data-mvcenter data-box&gt;&lt;div data-hcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;&lt;/div&gt;<br />
    &lt;div data-mvcenter data-box&gt;&lt;div data-vcenter data-box&gt;&lt;p data-center&gt;data-mvcenter&lt;/p&gt;&lt;/div&gt;&lt;/div&gt;<br />
    &lt;div data-mvcenter data-box&gt;&lt;div data-mhcenter&gt;&lt;/div&gt;&lt;div data-mhcenter&gt;&lt;/div&gt;&lt;/div&gt;<br />
&lt;/div&gt;
  </code>
</pre>
<div class="mvcenter" data-box>
	<div data-mvcenter data-box><div data-hcenter data-box><p data-center>data-hcenter</p></div></div>
    <div data-mvcenter data-box><div data-vcenter data-box><p data-center>data-vcenter</p></div></div>
    <div data-mvcenter data-box><div data-mhcenter></div><div data-mhcenter></div></div>
</div>
