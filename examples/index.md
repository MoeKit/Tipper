# 基本使用呀
---


````html
<style>
.button {
background: #494C51;
border-radius: 3px;
color: #fff;
cursor: pointer;
display: block;
font-family: 'Lato', sans-serif;
font-size: 14px;
height: 40px;
line-height: 40px;
margin: 0 0 10px 0;
text-align: center;
text-transform: uppercase;
-webkit-user-select: none;
-moz-user-select: none;
-ms-user-select: none;
-o-user-select: none;
user-select: none;
color:#fff;
}
			.tipped { background: #999; clear: both; float: none; display: block; margin: 20px auto; width: 50%; color:#fff; }
			.spmjs a.tipped {color:#fff;}
			.tipped:hover { background: #777; }
		</style>
<h2>Basic</h2>
<p>Tipper will generate a tooltip based on the target element's <code>data-title</code>. It can also be configured to open in multiple directions by passing the direction at initialization:</p>

<pre class="example"><code class="language-javascript">$(".target").tipper({
direction: "top"
});</code></pre>
<pre class="example"><code class="language-markup">&lt;a href="#" data-title="ToolTip Text"&gt;Tooltip Target&lt;/a&gt;</code></pre>

<h5>Demo</h5>
<div class="clear_fix">
    <a href="#" class="button tipped" data-title="Great New Tooltip" data-tipper-options='{"direction":"left"}'>Left</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip" data-tipper-options='{"direction":"right"}'>Right</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip" data-tipper-options='{"direction":"top"}'>Top</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip" data-tipper-options='{"direction":"bottom"}'>Bottom</a>
</div>

<br />

<!-- FOLLOW -->
<h2>Follow</h2>
<p>You can configure Tipper to follow the user's mouse:</p>

<pre class="example"><code class="language-javascript">$(".target").tipper({
follow: true
});</code></pre>

<h5>Demo</h5>
<div class="clear_fix">
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"left","follow":"true"}'>Left</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"right","follow":"true"}'>Right</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"top","follow":"true"}'>Top</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"bottom","follow":"true"}'>Bottom</a>
</div>

<br />

<!-- MATCH -->
<h2>Match</h2>
<p>You can configure Tipper to match the user's mouse position relative to the target:</p>

<pre class="example"><code class="language-javascript">$(".target").tipper({
match: true
});</code></pre>

<h5>Demo</h5>
<div class="clear_fix">
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"left","match":"true"}'>Left</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"right","match":"true"}'>Right</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"top","match":"true"}'>Top</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"bottom","match":"true"}'>Bottom</a>
</div>

<br />

<!-- DELAY -->
<h2>Delay</h2>
<p>You can set a delay to avoid accidental tooltips:</p>

<pre class="example"><code class="language-javascript">$(".target").tipper({
delay: 500
});</code></pre>

<h5>Demo</h5>
<div class="clear_fix">
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"left","delay":"500"}'>Left</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"right","delay":"500"}'>Right</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"top","delay":"500"}'>Top</a>
    <a href="#" class="button tipped" data-title="Great New Tooltip"  data-tipper-options='{"direction":"bottom","delay":"500"}'>Bottom</a>
</div>
````

````javascript
seajs.use('index',function($){
    $(".tipped").tipper();
})
````