
<div id="page"      style="display: none;"><!-- Bootstrap --></div>
<div id='home-url'  style="display: none;"><!-- http://www.jeffruss.com --></div>
<div id='logo-url'  style="display: none;"><!-- https://s3.amazonaws.com/shared-img-res/JR%20logo/JR_20px_wide.png --></div>

<div class="catergory-menu" id='HowTo'  style="display: none;"><!--  --></div>
<div class="catergory-menu" id='Resume' style="display: none;"><!--  --></div>
<div class="catergory-menu" id='GitHub' style="display: none;"><!--  --></div>

<div class="page-menu" id='Boostrap' style="display: none;"><!--http://www.jeffruss.com/?docs=bootstrap--></div>
<div class="page-menu" id='Rails'    style="display: none;"><!--http://www.jeffruss.com/?docs=rails--></div>

<!-- __________________________________________________________________ -->

# How-To: Bootstrap

----------------------------------------------------------------------------

## Bootstrap Basics

<div class="section" id='Grids'><!--#Grids--></div> 

### The Grid System

<br /><br />

#### 1. Grid Basics

----------------------------------------------------------------------------


<div class="container-fluid" style='outline: 1px solid orange; background-color:#404347'><br>
	<p>The orange border is there to show you that this is a div with the 
	bootstrap <code>container</code> class.</p><br>
	<div class="row"><br>
		<div class="col-xs-12" style='outline: 1px solid red' >
			<p>The red border is to reveal a div with the bootstrap row class 
			inside the container div.</p>
		</div>
	</div><br>
	<p>A row has a total of  width of 12 columns regardless of screen size.</p>
	<div class ="row"><br>
		<div class="col-xs-1" style="outline: 1px solid #20f030">1</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">2</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">3</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">4</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">5</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">6</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">7</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">8</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">9</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">10</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">11</div>
		<div class="col-xs-1" style="outline: 1px solid #20f030">12</div>
	</div><br>
	<div class="row">
		<div class="col-xs-6">
			<p>Each of the green boxes is a div with the class of <code>col-xs-1</code> which is one row. 
			These 12 divs are nested in single div with the class row, which is nested
			in a div with the class container. xs stands for an extra small screen as 
			in a mobile phone. The div's retain their status as being one column each 
			all the way down to the smallest screens. The arrangement will look the 
			same anywhere. see code:</p>
		</div>
		<div class="col-xs-6">
<xmp>
<div class="container">
	<div class ="row">
		<div class="col-xs-1">1</div>
		<div class="col-xs-1">2</div>
		<div class="col-xs-1">3</div>
		<div class="col-xs-1">4</div>
		<div class="col-xs-1">5</div>
		<div class="col-xs-1">6</div>
		<div class="col-xs-1">7</div>
		<div class="col-xs-1">8</div>
		<div class="col-xs-1">9</div>
		<div class="col-xs-1">10</div>
		<div class="col-xs-1">11</div>
		<div class="col-xs-1">12</div>
	</div>
</div>
</xmp>
		</div>
	</div>
</div>

<br /><br /><br />

#### 2. Grid Collapse

----------------------------------------------------------------------------

xs rows side by side on all screen sizes but if you specified lg instead of xs, 
the rows would collapse into being stacked vertically on any screen 
smaller than large screens, which is defined as 1170px wide. md would stack 
if less than 970px and sm would at 750px. Shrink the screen to watch these 
collapse:

<div class="container-fluid" style='outline: 2px solid orange; background-color:#404347'><br>
	<div class ="row">
		<div class="col-md-4" style="outline: 1px solid #20f030">col-md-4</div>
		<div class="col-md-4" style="outline: 1px solid #20f030">col-md-4</div>
		<div class="col-md-4" style="outline: 1px solid #20f030">col-md-4</div>
	</div>
</div>

<br /><br /><br />

#### 3. Adaptive Grids

----------------------------------------------------------------------------

<div class="container-fluid " style='outline: 1px solid orange; background-color:#404347'><br>
	<p>The div's below will size differently on different screen sizes because they 
	given multiple class attributes. Resize the screen to watch them change classes.</p>
	<br><br>
	<div class="row">
		<div class="col-xs-11 col-sm-9 col-md-3 col-lg-1" style="outline: 1px solid #20f030">I'm bigger on smaller screens</div>
		<div class="col-xs-1 col-sm-3 col-md-9 col-lg-11" style="outline: 1px solid #20f030" style='overflow: scroll'>I'm bigger on bigger screens</div>
	</div>
<xmp>
<div class="col-xs-11 col-sm-9 col-md-3 col-lg-1">I'm bigger on smaller screens</div>
<div class="col-xs-1 col-sm-3 col-md-9 col-lg-11">I'm bigger on bigger screens</div>
</xmp>
</div>

<br /><br /><br />

#### 4. Grid Offsets

----------------------------------------------------------------------------

<div class="container-fluid"  style='outline: 1px solid orange; background-color:#404347' ><br>
	<p>You can use offset to add a little empty space to the left. Add empty space 
	to the right side of the entire row simply by not adding up to 12 before closing 
	the div with the class row.</p><br><br>
	<div class="row">
		<div class="col-sm-4 col-sm-offset-2" style="outline: 1px solid #20f030">-> Offset by 2</div>
		<div class="col-sm-4 text-right" style="outline: 1px solid #20f030">there are two empty rows here -></div>
	</div>
	<xmp>
<div class="col-sm-4 col-sm-offset-2">-> Offset by 2</div>
<div class="col-sm-4 text-right">there are two empty rows here -></div>
	</xmp>
	<p>Note that <code>text-right</code> is a bootstrap class, along with <code>text-left</code> and 
	text-center</p>
	<br><br>
</div> 

<br /><br /><br />

### Jumbotron

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-xs-11  col-sm-11 col-sm-offset-1">
		<div class="jumbotron">
			<div class="container text-center">
				<h1>Jumbotron</h1>
				<p>A paragraph.</p>
			</div>
		</div>
	</div>
</div>
<div class='row'>
	<div class="col-sm-5 col-sm-offset-1">
		<br><br><p>To create a big banner area for a page or section title you can create a div with 
		the class <code>jumbotron</code>. If it is atop the page and you have a navbar, the navbar 
		will hide part of the jumbrotron. One fix is some inline CSS as you see  
		here. </p>
	</div>
	<div class="col-sm-6">
		<xmp>
	<style> body { padding-top 50px; } </style>		
	<div class="jumbotron">
		<div class="container text-center">
			<h1>Jumbotron</h1>
			<p>A paragraph.</p>
		</div>
	</div>
		</xmp>
	</div>
</div>

<br /><br /><br />

### Well

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-xs-6 col-sm-5 col-sm-offset-1">
		<div class="well">a well</div>
	</div>
	<div class="col-xs-6">
		<div class="well">a well</div>
	</div>
</div>
<div class='row'>
	<div class="col-sm-5 col-sm-offset-1">
		<br><br><p>A well is similar to jumbotron only much more subtle. It's meant 
		to give an element to give it an inset effect.</p>
	</div>
	<div class="col-sm-6">
		<xmp>
<div class="col-xs-6">
	<div class="well">a well</div>
</div>
<div class="col-xs-6">
	<div class="well">a well</div>
</div>
		</xmp>
	</div>
</div>


<div class="section jump" id='Buttons'><!--#Buttons--></div> 

----------------------------------------------------------------------------

## Buttons

----------------------------------------------------------------------------


<br /><br />

#### 1. Seven Colors

----------------------------------------------------------------------------

<div class="row"> 
	<div class="col-sm-11 col-sm-offset-1">
		<button type="button" class="btn btn-default">Default</button>
		<button type="button" class="btn btn-primary">Primary</button>
		<button type="button" class="btn btn-success">Success</button>
		<button type="button" class="btn btn-info">Info</button>
		<button type="button" class="btn btn-warning">Warning</button>
		<button type="button" class="btn btn-danger">Danger</button>
		<button type="button" class="btn btn-link">Link</button>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1"><br>
		<p>Below is the code for the above buttons. As you can see, bootstrap buttons 
		play nice with many different HTML elements. If inside a form, you would use 
		<code>type="submit"</code> rather than <code>type="button"</code></p>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<xmp>
<button type="button" class="btn btn-default">Default</button>
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-link">Link</button>
		</xmp>
	</div>
</div>

<br /><br /><br />

#### 2. As Links

----------------------------------------------------------------------------

<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<p>Buttons can also be in used for links using the anchor tag or used with the 
		<code>link_to</code> function in a Rails application:</p>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<xmp>
<a href="#" class="btn btn-default" role="button">GO!</a>
<%= link_to "GO!", bootstrap_home_path, class: 'btn btn-default' %>
		</xmp>
	</div> 
</div>

<br /><br /><br />

#### 3. Button Sizes

----------------------------------------------------------------------------

<div class="row"> 
	<div class="col-sm-11 col-sm-offset-1">
		<p>They are available in four different sizes:<p><br>
		<button type="button" class="btn btn-primary btn-lg">Large</button>
		<button type="button" class="btn btn-primary btn-md">Medium</button>
		<button type="button" class="btn btn-primary btn-sm">Small</button>
		<button type="button" class="btn btn-primary btn-xs">XSmall</button>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1"><br>
		<button type="button" class="btn btn-primary btn-lg">Large</button>
		<button type="button" class="btn btn-primary btn-md">Medium</button>
		<button type="button" class="btn btn-primary btn-sm">Small</button>
		<button type="button" class="btn btn-primary btn-xs">XSmall</button>        
	</div>
</div>

<br /><br /><br />

#### 4. Disabled Buttons

----------------------------------------------------------------------------
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<p>Buttons can be either active or disabled. The <code>active</code> class makes a button 
		be clickable, and the <code>disabled</code> class makes a button unavailable:<p><br><br>
		<button type="button" class="btn btn-primary active">Active Primary</button>
		<button type="button" class="btn btn-primary disabled">Disabled Primary</button>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<xmp>
<button type="button" class="btn btn-primary active">Active Primary</button>
<button type="button" class="btn btn-primary disabled">Disabled Primary</button> 
		</xmp>
	</div>
</div>

<br /><br /><br />

#### 5. Transparent Buttons

----------------------------------------------------------------------------

<div class="row"> 
	<div class="col-sm-11 col-sm-offset-1">
		<p>Although not part of bootstrap, you can get transparent buttons by using a 
		little CSS.</p><br>
		<button type="button" class="btn btn-default btn-ghost">Default</button>
		<button type="button" class="btn btn-primary btn-ghost">Primary</button>
		<button type="button" class="btn btn-success btn-ghost">Success</button>
		<button type="button" class="btn btn-info btn-ghost">Info</button>
		<button type="button" class="btn btn-warning btn-ghost">Warning</button>
		<button type="button" class="btn btn-danger btn-ghost">Danger</button>
	</div>
</div>

<div class="row"> 
	<div class="col-sm-11 col-sm-offset-1">
		<p><br><br>this was done by adding the class <code>btn-ghost</code> 
		which can be defined like this:</p>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1"><br>	
		<xmp>
.btn-ghost{
background: transparent !important;
color: #F2F2F2 !important;

/* CSS Transition */
-webkit-transition: background .2s ease-in-out, border .2s ease-in-out;
-moz-transition: background .2s ease-in-out, border .2s ease-in-out;
-ms-transition: background .2s ease-in-out, border .2s ease-in-out;
-o-transition: background .2s ease-in-out, border .2s ease-in-out;
transition: background .2s ease-in-out, border .2s ease-in-out;
}       
		</xmp>
	</div>
</div>

<br /><br /><br />

#### 6. Block Level Buttons

----------------------------------------------------------------------------

<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<p>Normally a button will expand and contract to accomodate the contents 
		inside it. A button with the class <code>btn-block</code> will span the entire width of the 
		parent element.</p><br>
		<button type="button" class="btn btn-primary btn-block">Button 1</button>
		<br>
		<xmp>
<button type="button" class="btn btn-primary btn-block">Button 1</button>
		</xmp>
	</div>
</div>

<br /><br /><br />

#### 7. Button Groups 

----------------------------------------------------------------------------

<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1">
		<p>You can effect the appearance and spacing of buttons by grouping them together. 
		To do this, simply wrap your buttons in a div with the class <code>btn-group</code>.</p><br>
		<div class="btn-group">
			<button type="button" class="btn btn-success btn-lg">BUY NOW!</button>
			<button type="button" class="btn btn-primary btn-lg">get for free</button>
		</div>
	</div>
</div>
<div class="row"> 
	<div class="col-sm-8 col-sm-offset-1"><br>
		<xmp>
<div class="btn-group">
	<button type="button" class="btn btn-success btn-lg">BUY NOW!</button>
	<button type="button" class="btn btn-primary btn-lg">get for free</button>
</div>
		</xmp>
	</div>
</div>


<br /><br /><br />

<div class="section jump" id='Glyphs'><!--#Glyphs--></div> 

----------------------------------------------------------------------------

## Glyph Icons

----------------------------------------------------------------------------


<div class="row">
	<div class="col-xs-10 col-xs-offset-1">  
	</p>Glyphicons are icon fonts which are preverable to images as a means of 
	creating icons because they are scalable.</p>
	</div>
</div><br>

<div class="row">
	<div class="col-xs-6">  
		<span class="glyphicon glyphicon-asterisk"></span> glyphicon glyphicon-asterisk<br>
		<span class="glyphicon glyphicon-plus"></span> glyphicon glyphicon-plus<br>
		<span class="glyphicon glyphicon-minus"></span> glyphicon glyphicon-minus<br>
		<span class="glyphicon glyphicon-euro"></span> glyphicon glyphicon-euro<br>
		<span class="glyphicon glyphicon-cloud"></span> glyphicon glyphicon-cloud<br>
		<span class="glyphicon glyphicon-envelope"></span> glyphicon glyphicon-envelope<br>
		<span class="glyphicon glyphicon-pencil"></span> glyphicon glyphicon-pencil<br>
		<span class="glyphicon glyphicon-glass"></span> glyphicon glyphicon-glass<br>
		<span class="glyphicon glyphicon-music"></span> glyphicon glyphicon-music<br>
		<span class="glyphicon glyphicon-search"></span> glyphicon glyphicon-search<br>
		<span class="glyphicon glyphicon-heart"></span> glyphicon glyphicon-heart<br>
		<span class="glyphicon glyphicon-star"></span> glyphicon glyphicon-star<br>
		<span class="glyphicon glyphicon-star-empty"></span> glyphicon glyphicon-star-empty<br>
		<span class="glyphicon glyphicon-user"></span> glyphicon glyphicon-user<br>
		<span class="glyphicon glyphicon-film"></span> glyphicon glyphicon-film<br>
		<span class="glyphicon glyphicon-th-large"></span> glyphicon glyphicon-th-large<br>
		<span class="glyphicon glyphicon-th"></span> glyphicon glyphicon-th<br>
		<span class="glyphicon glyphicon-th-list"></span> glyphicon glyphicon-th-list<br>
		<span class="glyphicon glyphicon-ok"></span> glyphicon glyphicon-ok<br>
		<span class="glyphicon glyphicon-remove"></span> glyphicon glyphicon-remove<br>
		<span class="glyphicon glyphicon-zoom-in"></span> glyphicon glyphicon-zoom-in<br>
		<span class="glyphicon glyphicon-zoom-out"></span> glyphicon glyphicon-zoom-out<br>
		<span class="glyphicon glyphicon-off"></span> glyphicon glyphicon-off<br>
		<span class="glyphicon glyphicon-signal"></span> glyphicon glyphicon-signal<br>
		<span class="glyphicon glyphicon-cog"></span> glyphicon glyphicon-cog<br>
		<span class="glyphicon glyphicon-trash"></span> glyphicon glyphicon-trash<br>
		<span class="glyphicon glyphicon-home"></span> glyphicon glyphicon-home<br>
		<span class="glyphicon glyphicon-file"></span> glyphicon glyphicon-file<br>
		<span class="glyphicon glyphicon-time"></span> glyphicon glyphicon-time<br>
		<span class="glyphicon glyphicon-road"></span> glyphicon glyphicon-road<br>
		<span class="glyphicon glyphicon-download-alt"></span> glyphicon glyphicon-download-alt<br>
		<span class="glyphicon glyphicon-download"></span> glyphicon glyphicon-download<br>
		<span class="glyphicon glyphicon-upload"></span> glyphicon glyphicon-upload<br>
		<span class="glyphicon glyphicon-inbox"></span> glyphicon glyphicon-inbox<br>
		<span class="glyphicon glyphicon-play-circle"></span> glyphicon glyphicon-play-circle<br>
		<span class="glyphicon glyphicon-repeat"></span> glyphicon glyphicon-repeat<br>
		<span class="glyphicon glyphicon-refresh"></span> glyphicon glyphicon-refresh<br>
		<span class="glyphicon glyphicon-list-alt"></span> glyphicon glyphicon-list-alt<br>
		<span class="glyphicon glyphicon-lock"></span> glyphicon glyphicon-lock<br>
		<span class="glyphicon glyphicon-flag"></span> glyphicon glyphicon-flag<br>
		<span class="glyphicon glyphicon-headphones"></span> glyphicon glyphicon-headphones<br>
		<span class="glyphicon glyphicon-volume-off"></span> glyphicon glyphicon-volume-off<br>
		<span class="glyphicon glyphicon-volume-down"></span> glyphicon glyphicon-volume-down<br>
		<span class="glyphicon glyphicon-volume-up"></span> glyphicon glyphicon-volume-up<br>
		<span class="glyphicon glyphicon-qrcode"></span> glyphicon glyphicon-qrcode<br>
		<span class="glyphicon glyphicon-barcode"></span> glyphicon glyphicon-barcode<br>
		<span class="glyphicon glyphicon-tag"></span> glyphicon glyphicon-tag<br>
		<span class="glyphicon glyphicon-tags"></span> glyphicon glyphicon-tags<br>
		<span class="glyphicon glyphicon-book"></span> glyphicon glyphicon-book<br>
		<span class="glyphicon glyphicon-bookmark"></span> glyphicon glyphicon-bookmark<br>
		<span class="glyphicon glyphicon-print"></span> glyphicon glyphicon-print<br>
		<span class="glyphicon glyphicon-camera"></span> glyphicon glyphicon-camera<br>
		<span class="glyphicon glyphicon-font"></span> glyphicon glyphicon-font<br>
		<span class="glyphicon glyphicon-bold"></span> glyphicon glyphicon-bold<br>
		<span class="glyphicon glyphicon-italic"></span> glyphicon glyphicon-italic<br>
		<span class="glyphicon glyphicon-text-height"></span> glyphicon glyphicon-text-height<br>
		<span class="glyphicon glyphicon-text-width"></span> glyphicon glyphicon-text-width<br>
		<span class="glyphicon glyphicon-align-left"></span> glyphicon glyphicon-align-left<br>
		<span class="glyphicon glyphicon-align-center"></span> glyphicon glyphicon-align-center<br>
		<span class="glyphicon glyphicon-align-right"></span> glyphicon glyphicon-align-right<br>
		<span class="glyphicon glyphicon-align-justify"></span> glyphicon glyphicon-align-justify<br>
		<span class="glyphicon glyphicon-list"></span> glyphicon glyphicon-list<br>
		<span class="glyphicon glyphicon-indent-left"></span> glyphicon glyphicon-indent-left<br>
		<span class="glyphicon glyphicon-indent-right"></span> glyphicon glyphicon-indent-right<br>
		<span class="glyphicon glyphicon-facetime-video"></span> glyphicon glyphicon-facetime-video<br>
		<span class="glyphicon glyphicon-picture"></span> glyphicon glyphicon-picture<br>
		<span class="glyphicon glyphicon-map-marker"></span> glyphicon glyphicon-map-marker<br>
		<span class="glyphicon glyphicon-adjust"></span> glyphicon glyphicon-adjust<br>
		<span class="glyphicon glyphicon-tint"></span> glyphicon glyphicon-tint<br>
		<span class="glyphicon glyphicon-edit"></span> glyphicon glyphicon-edit<br>
		<span class="glyphicon glyphicon-share"></span> glyphicon glyphicon-share<br>
		<span class="glyphicon glyphicon-check"></span> glyphicon glyphicon-check<br>
		<span class="glyphicon glyphicon-move"></span> glyphicon glyphicon-move<br>
		<span class="glyphicon glyphicon-step-backward"></span> glyphicon glyphicon-step-backward<br>
		<span class="glyphicon glyphicon-fast-backward"></span> glyphicon glyphicon-fast-backward<br>
		<span class="glyphicon glyphicon-backward"></span> glyphicon glyphicon-backward<br>
		<span class="glyphicon glyphicon-play"></span> glyphicon glyphicon-play<br>
		<span class="glyphicon glyphicon-pause"></span> glyphicon glyphicon-pause<br>
		<span class="glyphicon glyphicon-stop"></span> glyphicon glyphicon-stop<br>
		<span class="glyphicon glyphicon-forward"></span> glyphicon glyphicon-forward<br>
		<span class="glyphicon glyphicon-fast-forward"></span> glyphicon glyphicon-fast-forward<br>
		<span class="glyphicon glyphicon-step-forward"></span> glyphicon glyphicon-step-forward<br>
		<span class="glyphicon glyphicon-eject"></span> glyphicon glyphicon-eject<br>
		<span class="glyphicon glyphicon-chevron-left"></span> glyphicon glyphicon-chevron-left<br>
		<span class="glyphicon glyphicon-chevron-right"></span> glyphicon glyphicon-chevron-right<br>
		<span class="glyphicon glyphicon-plus-sign"></span> glyphicon glyphicon-plus-sign<br>
		<span class="glyphicon glyphicon-minus-sign"></span> glyphicon glyphicon-minus-sign<br>
		<span class="glyphicon glyphicon-remove-sign"></span> glyphicon glyphicon-remove-sign<br>
		<span class="glyphicon glyphicon-ok-sign"></span> glyphicon glyphicon-ok-sign<br>
		<span class="glyphicon glyphicon-question-sign"></span> glyphicon glyphicon-question-sign<br>
		<span class="glyphicon glyphicon-info-sign"></span> glyphicon glyphicon-info-sign<br>
		<span class="glyphicon glyphicon-screenshot"></span> glyphicon glyphicon-screenshot<br>
		<span class="glyphicon glyphicon-remove-circle"></span> glyphicon glyphicon-remove-circle<br>
		<span class="glyphicon glyphicon-ok-circle"></span> glyphicon glyphicon-ok-circle<br>
		<span class="glyphicon glyphicon-ban-circle"></span> glyphicon glyphicon-ban-circle<br>
		<span class="glyphicon glyphicon-arrow-left"></span> glyphicon glyphicon-arrow-left<br>
		<span class="glyphicon glyphicon-arrow-right"></span> glyphicon glyphicon-arrow-right<br>
		<span class="glyphicon glyphicon-arrow-up"></span> glyphicon glyphicon-arrow-up<br>
		<span class="glyphicon glyphicon-arrow-down"></span> glyphicon glyphicon-arrow-down<br>
		<span class="glyphicon glyphicon-share-alt"></span> glyphicon glyphicon-share-alt<br>
		<span class="glyphicon glyphicon-resize-full"></span> glyphicon glyphicon-resize-full<br>
		<span class="glyphicon glyphicon-resize-small"></span> glyphicon glyphicon-resize-small<br>
		<span class="glyphicon glyphicon-exclamation-sign"></span> glyphicon glyphicon-exclamation-sign<br>
		<span class="glyphicon glyphicon-gift"></span> glyphicon glyphicon-gift<br>
		<span class="glyphicon glyphicon-leaf"></span> glyphicon glyphicon-leaf<br>
		<span class="glyphicon glyphicon-fire"></span> glyphicon glyphicon-fire<br>
		<span class="glyphicon glyphicon-eye-open"></span> glyphicon glyphicon-eye-open<br>
		<span class="glyphicon glyphicon-eye-close"></span> glyphicon glyphicon-eye-close<br>
		<span class="glyphicon glyphicon-warning-sign"></span> glyphicon glyphicon-warning-sign<br>
		<span class="glyphicon glyphicon-plane"></span> glyphicon glyphicon-plane<br>
		<span class="glyphicon glyphicon-calendar"></span> glyphicon glyphicon-calendar<br>
		<span class="glyphicon glyphicon-random"></span> glyphicon glyphicon-random<br>
		<span class="glyphicon glyphicon-comment"></span> glyphicon glyphicon-comment<br>
		<span class="glyphicon glyphicon-magnet"></span> glyphicon glyphicon-magnet<br>
		<span class="glyphicon glyphicon-chevron-up"></span> glyphicon glyphicon-chevron-up<br>
		<span class="glyphicon glyphicon-chevron-down"></span> glyphicon glyphicon-chevron-down<br>
		<span class="glyphicon glyphicon-retweet"></span> glyphicon glyphicon-retweet<br>
		<span class="glyphicon glyphicon-shopping-cart"></span> glyphicon glyphicon-shopping-cart<br>
		<span class="glyphicon glyphicon-folder-close"></span> glyphicon glyphicon-folder-close<br>
		<span class="glyphicon glyphicon-folder-open"></span> glyphicon glyphicon-folder-open<br>
		<span class="glyphicon glyphicon-resize-vertical"></span> glyphicon glyphicon-resize-vertical<br>
		<span class="glyphicon glyphicon-resize-horizontal"></span> glyphicon glyphicon-resize-horizontal<br>
		<span class="glyphicon glyphicon-hdd"></span> glyphicon glyphicon-hdd<br>
		<span class="glyphicon glyphicon-bullhorn"></span> glyphicon glyphicon-bullhorn<br>
		<span class="glyphicon glyphicon-bell"></span> glyphicon glyphicon-bell<br>
		<span class="glyphicon glyphicon-certificate"></span> glyphicon glyphicon-certificate<br>
		<span class="glyphicon glyphicon-thumbs-up"></span> glyphicon glyphicon-thumbs-up<br>
		<span class="glyphicon glyphicon-thumbs-down"></span> glyphicon glyphicon-thumbs-down<br>
	</div>
	<div class="col-xs-6">  
		<span class="glyphicon glyphicon-hand-right"></span> glyphicon glyphicon-hand-right<br>
		<span class="glyphicon glyphicon-hand-left"></span> glyphicon glyphicon-hand-left<br>
		<span class="glyphicon glyphicon-hand-up"></span> glyphicon glyphicon-hand-up<br>
		<span class="glyphicon glyphicon-hand-down"></span> glyphicon glyphicon-hand-down<br>
		<span class="glyphicon glyphicon-circle-arrow-right"></span> glyphicon glyphicon-circle-arrow-right<br>
		<span class="glyphicon glyphicon-circle-arrow-left"></span> glyphicon glyphicon-circle-arrow-left<br>
		<span class="glyphicon glyphicon-circle-arrow-up"></span> glyphicon glyphicon-circle-arrow-up<br>
		<span class="glyphicon glyphicon-circle-arrow-down"></span> glyphicon glyphicon-circle-arrow-down<br>
		<span class="glyphicon glyphicon-globe"></span> glyphicon glyphicon-globe<br>
		<span class="glyphicon glyphicon-wrench"></span> glyphicon glyphicon-wrench<br>
		<span class="glyphicon glyphicon-tasks"></span> glyphicon glyphicon-tasks<br>
		<span class="glyphicon glyphicon-filter"></span> glyphicon glyphicon-filter<br>
		<span class="glyphicon glyphicon-briefcase"></span> glyphicon glyphicon-briefcase<br>
		<span class="glyphicon glyphicon-fullscreen"></span> glyphicon glyphicon-fullscreen<br>
		<span class="glyphicon glyphicon-dashboard"></span> glyphicon glyphicon-dashboard<br>
		<span class="glyphicon glyphicon-paperclip"></span> glyphicon glyphicon-paperclip<br>
		<span class="glyphicon glyphicon-heart-empty"></span> glyphicon glyphicon-heart-empty<br>
		<span class="glyphicon glyphicon-link"></span> glyphicon glyphicon-link<br>
		<span class="glyphicon glyphicon-phone"></span> glyphicon glyphicon-phone<br>
		<span class="glyphicon glyphicon-pushpin"></span> glyphicon glyphicon-pushpin<br>
		<span class="glyphicon glyphicon-usd"></span> glyphicon glyphicon-usd<br>
		<span class="glyphicon glyphicon-gbp"></span> glyphicon glyphicon-gbp<br>
		<span class="glyphicon glyphicon-sort"></span> glyphicon glyphicon-sort<br>
		<span class="glyphicon glyphicon-sort-by-alphabet"></span> glyphicon glyphicon-sort-by-alphabet<br>
		<span class="glyphicon glyphicon-sort-by-alphabet-alt"></span> glyphicon glyphicon-sort-by-alphabet-alt<br>
		<span class="glyphicon glyphicon-sort-by-order"></span> glyphicon glyphicon-sort-by-order<br>
		<span class="glyphicon glyphicon-sort-by-order-alt"></span> glyphicon glyphicon-sort-by-order-alt<br>
		<span class="glyphicon glyphicon-sort-by-attributes"></span> glyphicon glyphicon-sort-by-attributes<br>
		<span class="glyphicon glyphicon-sort-by-attributes-alt"></span> glyphicon glyphicon-sort-by-attributes-alt<br>
		<span class="glyphicon glyphicon-unchecked"></span> glyphicon glyphicon-unchecked<br>
		<span class="glyphicon glyphicon-expand"></span> glyphicon glyphicon-expand<br>
		<span class="glyphicon glyphicon-collapse-down"></span> glyphicon glyphicon-collapse-down<br>
		<span class="glyphicon glyphicon-collapse-up"></span> glyphicon glyphicon-collapse-up<br>
		<span class="glyphicon glyphicon-log-in"></span> glyphicon glyphicon-log-in<br>
		<span class="glyphicon glyphicon-flash"></span> glyphicon glyphicon-flash<br>
		<span class="glyphicon glyphicon-log-out"></span> glyphicon glyphicon-log-out<br>
		<span class="glyphicon glyphicon-new-window"></span> glyphicon glyphicon-new-window<br>
		<span class="glyphicon glyphicon-record"></span> glyphicon glyphicon-record<br>
		<span class="glyphicon glyphicon-save"></span> glyphicon glyphicon-save<br>
		<span class="glyphicon glyphicon-open"></span> glyphicon glyphicon-open<br>
		<span class="glyphicon glyphicon-saved"></span> glyphicon glyphicon-saved<br>
		<span class="glyphicon glyphicon-import"></span> glyphicon glyphicon-import<br>
		<span class="glyphicon glyphicon-export"></span> glyphicon glyphicon-export<br>
		<span class="glyphicon glyphicon-send"></span> glyphicon glyphicon-send<br>
		<span class="glyphicon glyphicon-floppy-disk"></span> glyphicon glyphicon-floppy-disk<br>
		<span class="glyphicon glyphicon-floppy-saved"></span> glyphicon glyphicon-floppy-saved<br>
		<span class="glyphicon glyphicon-floppy-remove"></span> glyphicon glyphicon-floppy-remove<br>
		<span class="glyphicon glyphicon-floppy-save"></span> glyphicon glyphicon-floppy-save<br>
		<span class="glyphicon glyphicon-floppy-open"></span> glyphicon glyphicon-floppy-open<br>
		<span class="glyphicon glyphicon-credit-card"></span> glyphicon glyphicon-credit-card<br>
		<span class="glyphicon glyphicon-transfer"></span> glyphicon glyphicon-transfer<br>
		<span class="glyphicon glyphicon-cutlery"></span> glyphicon glyphicon-cutlery<br>
		<span class="glyphicon glyphicon-header"></span> glyphicon glyphicon-header<br>
		<span class="glyphicon glyphicon-compressed"></span> glyphicon glyphicon-compressed<br>
		<span class="glyphicon glyphicon-earphone"></span> glyphicon glyphicon-earphone<br>
		<span class="glyphicon glyphicon-phone-alt"></span> glyphicon glyphicon-phone-alt<br>
		<span class="glyphicon glyphicon-tower"></span> glyphicon glyphicon-tower<br>
		<span class="glyphicon glyphicon-stats"></span> glyphicon glyphicon-stats<br>
		<span class="glyphicon glyphicon-sd-video"></span> glyphicon glyphicon-sd-video<br>
		<span class="glyphicon glyphicon-hd-video"></span> glyphicon glyphicon-hd-video<br>
		<span class="glyphicon glyphicon-subtitles"></span> glyphicon glyphicon-subtitles<br>
		<span class="glyphicon glyphicon-sound-stereo"></span> glyphicon glyphicon-sound-stereo<br>
		<span class="glyphicon glyphicon-sound-dolby"></span> glyphicon glyphicon-sound-dolby<br>
		<span class="glyphicon glyphicon-sound-5-1"></span> glyphicon glyphicon-sound-5-1<br>
		<span class="glyphicon glyphicon-sound-6-1"></span> glyphicon glyphicon-sound-6-1<br>
		<span class="glyphicon glyphicon-sound-7-1"></span> glyphicon glyphicon-sound-7-1<br>
		<span class="glyphicon glyphicon-copyright-mark"></span> glyphicon glyphicon-copyright-mark<br>
		<span class="glyphicon glyphicon-registration-mark"></span> glyphicon glyphicon-registration-mark<br>
		<span class="glyphicon glyphicon-cloud-download"></span> glyphicon glyphicon-cloud-download<br>
		<span class="glyphicon glyphicon-cloud-upload"></span> glyphicon glyphicon-cloud-upload<br>
		<span class="glyphicon glyphicon-tree-conifer"></span> glyphicon glyphicon-tree-conifer<br>
		<span class="glyphicon glyphicon-tree-deciduous"></span> glyphicon glyphicon-tree-deciduous<br>
		<span class="glyphicon glyphicon-cd"></span> glyphicon glyphicon-cd<br>
		<span class="glyphicon glyphicon-save-file"></span> glyphicon glyphicon-save-file<br>
		<span class="glyphicon glyphicon-open-file"></span> glyphicon glyphicon-open-file<br>
		<span class="glyphicon glyphicon-level-up"></span> glyphicon glyphicon-level-up<br>
		<span class="glyphicon glyphicon-copy"></span> glyphicon glyphicon-copy<br>
		<span class="glyphicon glyphicon-paste"></span> glyphicon glyphicon-paste<br>
		<span class="glyphicon glyphicon-alert"></span> glyphicon glyphicon-alert<br>
		<span class="glyphicon glyphicon-equalizer"></span> glyphicon glyphicon-equalizer<br>
		<span class="glyphicon glyphicon-king"></span> glyphicon glyphicon-king<br>
		<span class="glyphicon glyphicon-queen"></span> glyphicon glyphicon-queen<br>
		<span class="glyphicon glyphicon-pawn"></span> glyphicon glyphicon-pawn<br>
		<span class="glyphicon glyphicon-bishop"></span> glyphicon glyphicon-bishop<br>
		<span class="glyphicon glyphicon-knight"></span> glyphicon glyphicon-knight<br>
		<span class="glyphicon glyphicon-baby-formula"></span> glyphicon glyphicon-baby-formula<br>
		<span class="glyphicon glyphicon-tent"></span> glyphicon glyphicon-tent<br>
		<span class="glyphicon glyphicon-blackboard"></span> glyphicon glyphicon-blackboard<br>
		<span class="glyphicon glyphicon-bed"></span> glyphicon glyphicon-bed<br>
		<span class="glyphicon glyphicon-apple"></span> glyphicon glyphicon-apple<br>
		<span class="glyphicon glyphicon-erase"></span> glyphicon glyphicon-erase<br>
		<span class="glyphicon glyphicon-hourglass"></span> glyphicon glyphicon-hourglass<br>
		<span class="glyphicon glyphicon-lamp"></span> glyphicon glyphicon-lamp<br>
		<span class="glyphicon glyphicon-duplicate"></span> glyphicon glyphicon-duplicate<br>
		<span class="glyphicon glyphicon-piggy-bank"></span> glyphicon glyphicon-piggy-bank<br>
		<span class="glyphicon glyphicon-scissors"></span> glyphicon glyphicon-scissors<br>
		<span class="glyphicon glyphicon-bitcoin"></span> glyphicon glyphicon-bitcoin<br>
		<span class="glyphicon glyphicon-yen"></span> glyphicon glyphicon-yen<br>
		<span class="glyphicon glyphicon-ruble"></span> glyphicon glyphicon-ruble<br>
		<span class="glyphicon glyphicon-scale"></span> glyphicon glyphicon-scale<br>
		<span class="glyphicon glyphicon-ice-lolly"></span> glyphicon glyphicon-ice-lolly<br>
		<span class="glyphicon glyphicon-ice-lolly-tasted"></span> glyphicon glyphicon-ice-lolly-tasted<br>
		<span class="glyphicon glyphicon-education"></span> glyphicon glyphicon-education<br>
		<span class="glyphicon glyphicon-option-horizontal"></span> glyphicon glyphicon-option-horizontal<br>
		<span class="glyphicon glyphicon-option-vertical"></span> glyphicon glyphicon-option-vertical<br>
		<span class="glyphicon glyphicon-menu-hamburger"></span> glyphicon glyphicon-menu-hamburger<br>
		<span class="glyphicon glyphicon-modal-window"></span> glyphicon glyphicon-modal-window<br>
		<span class="glyphicon glyphicon-oil"></span> glyphicon glyphicon-oil<br>
		<span class="glyphicon glyphicon-grain"></span> glyphicon glyphicon-grain<br>
		<span class="glyphicon glyphicon-sunglasses"></span> glyphicon glyphicon-sunglasses<br>
		<span class="glyphicon glyphicon-text-size"></span> glyphicon glyphicon-text-size<br>
		<span class="glyphicon glyphicon-text-color"></span> glyphicon glyphicon-text-color<br>
		<span class="glyphicon glyphicon-text-background"></span> glyphicon glyphicon-text-background<br>
		<span class="glyphicon glyphicon-object-align-top"></span> glyphicon glyphicon-object-align-top<br>
		<span class="glyphicon glyphicon-object-align-bottom"></span> glyphicon glyphicon-object-align-bottom<br>
		<span class="glyphicon glyphicon-object-align-horizontal"></span> glyphicon glyphicon-object-align-horizontal<br>
		<span class="glyphicon glyphicon-object-align-left"></span> glyphicon glyphicon-object-align-left<br>
		<span class="glyphicon glyphicon-object-align-vertical"></span> glyphicon glyphicon-object-align-vertical<br>
		<span class="glyphicon glyphicon-object-align-right"></span> glyphicon glyphicon-object-align-right<br>
		<span class="glyphicon glyphicon-triangle-right"></span> glyphicon glyphicon-triangle-right<br>
		<span class="glyphicon glyphicon-triangle-left"></span> glyphicon glyphicon-triangle-left<br>
		<span class="glyphicon glyphicon-triangle-bottom"></span> glyphicon glyphicon-triangle-bottom<br>
		<span class="glyphicon glyphicon-triangle-top"></span> glyphicon glyphicon-triangle-top<br>
		<span class="glyphicon glyphicon-superscript"></span> glyphicon glyphicon-superscript<br>
		<span class="glyphicon glyphicon-subscript"></span> glyphicon glyphicon-subscript<br>
		<span class="glyphicon glyphicon-menu-left"></span> glyphicon glyphicon-menu-left<br>
		<span class="glyphicon glyphicon-menu-right"></span> glyphicon glyphicon-menu-right<br>
		<span class="glyphicon glyphicon-menu-down"></span> glyphicon glyphicon-menu-down<br>
		<span class="glyphicon glyphicon-menu-up"></span> glyphicon glyphicon-menu-up
	</div>
</div>


<br /><br /><br />

<div class="section jump" id='Forms'><!--#Forms--></div> 

--------------------------------------------------------------------------------

## FORMS

--------------------------------------------------------------------------------


<br /><br />

#### 1. Plain HTML forms

----------------------------------------------------------------------------

<div class="row">
    <div class="col-sm-9 col-sm-offset-1">
        <p>Basic HTML form look like below. To be submitted correctly, each input field 
        must have a <code>name</code> attribute.</p><br>
    </div>
</div>
<div class="row">
    <div class="col-xs-5 col-sm-2 col-xs-offset-1" style="color:grey">
        <form>
            <fieldset>
                <legend style="color:grey">Personal information:</legend>
                Enter first name:<br>
                <input type='text' name="firstname"><br>
                Enter last name:<br>
                <input type='text' name="lastname"><br>
                <input type="radio" name="sex" value="male" checked>Male<br>
                <input type="radio" name="sex" value="female">Female<br>
                <input type="checkbox" name="remember" value="remember" checked> Remember me<br>
                <input type="submit" value="Submit">
            </fieldset>
        </form>
    </div>
    <div class="col-xs-12 col-sm-8 col-sm-offset-1">
        <xmp>
<form action='action_page.php' method="post">
    <fieldset>
        <legend>Personal information:</legend>
        Enter first name:<br>
        <input type='text' name="firstname"><br>
        Enter last name:<br>
        <input type='text' name="lastname"><br>
        <input type="radio" name="sex" 
                value="male" checked>Male<br>
        <input type="radio" name="sex" 
                value="female">Female<br>
        <input type="submit" value="Submit">
    </fieldset>  
</form>  
        </xmp>
    </div><div class="col-xs-3"></div>
</div>

<br /><br />

#### 2. Basic Bootstrap Forms

----------------------------------------------------------------------------

<div class="row"> 
    <div class="col-xs-5 col-xs-4 col-sm-offset-1">
        <form action='' role='form'>
            <fieldset>
                <legend style="color:grey">Personal information:</legend>
                <div class='form-group'>
                    <label for='firstname'>First name:</label>
                    <input type='text' id='firstname' class='form-control'>
                </div>
                <div class='form-group'>
                    <label for='lastname'>Last name:</label>
                    <input type='text' id='lastname' class='form-control'>
                </div>
                <div class="radio">
                    <label><input type="radio" name="optradio">Male</label>
                </div>
                <div class="radio">
                    <label><input type="radio" name="optradio">Female</label>
                </div>
                <div class="checkbox">
                    <label><input type="checkbox"> Remember me</label>
                </div>
                <button type="submit" class="btn btn-default">Submit</button>
            <fieldset>
        </form> 
    </div>
    <div class="col-xm-4 col-xm-offset-1">
        <br><br><p>In Boostrap, our form block will have the <code>role='form'</code> and each form element 
        will be wrapped in separate div's with the exception of the submit button. 
        Text field elements have div's with a <code>class='form-group'</code>. The labels are  
        wrapped in label tags with <code>for='the_id'</code>. The input for the text fields have 
        matching id's and a class of <code>form-control</code>. Text field's div's carry the class 
        <code>form-group</code> but radio buttons have the <code>radio</code> class and checkboxes have the  
        <code>checkbox</code> class. Buttons need not be wrapped in div's but rather they are put 
        in button elements with <code>type="submit"</code>.</p><br>
    </div> 
</div>

<br /><br />

    <form action='action_page.php' role='form'>
        <fieldset>
            <legend style="color:grey">Personal information:</legend>
            <div class='form-group'>
                <label for='firstname'>First name:</label>
                <input type='text' id='firstname' class='form-control'>
            </div>
            <div class='form-group'>
                <label for='lastname'>Last name:</label>
                <input type='text' id='lastname' class='form-control'>
            </div>
            <div class="radio">
                <label><input type="radio" name="optradio">Male</label>
            </div>
            <div class="radio">
                <label><input type="radio" name="optradio">Female</label>
            </div>
            <div class="checkbox">
                <label><input type="checkbox"> Remember me</label>
            </div>
            <button type="submit" class="btn btn-default">Submit</button>
        </fieldset>
    </form>



<div class="row"> 
    <div class="col-sm-9 col-sm-offset-1"><br><br>
        <p>If you want some help text below an input field you can insure it's styled
        by using a p tag with the class <code>help-block</code>.</p><br>
    </div><div class='col-xs-4'></div>
</div>
<div class="row">       
    <div class="col-xs-7 col-sm-7 col-xs-offset-1">
        <form action='' role='form'>
                <div class='form-group'>
                    <label for='firstname'>First name:</label>
                    <input type='text' id='firstname' class='form-control'>
                    <p class='help-block'>What mommy and daddy call you.</p>
                </div>
        </form>    
    </div>
</div>

    <form action='' role='form'>
        <div class='form-group'>
            <label for='firstname'>First name:</label>
            <input type='text' id='firstname' class='form-control'>
            <p class='help-block'>What mommy and daddy call you.</p>
        </div>
    </form>   




<br /><br />

#### 3. Inline Forms:

----------------------------------------------------------------------------


<div class="row"> 
    <div class="col-sm-9 col-sm-offset-1"><br>
        <form action='' role='form' class='form-inline'>
            <div class='form-group'>
                <label for='username' class='sr-only'>User Name:</label>
                <input type='text' id='username' 
                        class='form-control' placeholder="Username or Email">
            </div>
            <div class='form-group'>
                <label for='password' class='sr-only'>Password:</label>
                <input type='password' id='password' 
                        class='form-control' placeholder='Password'>
            </div>
            <button type="submit" class="btn btn-default">Submit</button>
            <div class="checkbox">
                <label><input type="checkbox"> Remember me</label>
            </div>
        </form>    
    </div>
</div>
<div class="row">
    <div class="col-xs-11 col-sm-offset-1"><br> 
        <p>You can make the forms line up in a horizontal row by adding the class
        <code>form-inline</code> to the form element. With this style is customary to not use 
        labels, although we will have them show with screen readers by adding the 
        <code>sr-only</code> class.</p> 
    </div>
</div>
<div class="row">
    <div class="col-xs-12 col-sm-3 col-sm-offset-1"><br>
        <p>Instead of labels we will use placeholders by adding the 
        <code>placeholder</code> attribute with the value of the desired text for each input 
        element. <br><br>
        Notice that the input type for password is <code>password</code>, not <code>text</code>. This 
        insures the digits will not be visible on the screen.</p><br>
    </div>
    <div class="col-xs-12 col-sm-8">
        <xmp>
<form action='' role='form' class='form-inline'>
    <div class='form-group'>
        <label for='username' class='sr-only'>User Name:</label>
        <input type='text' id='username' 
                class='form-control' placeholder="Username or Email">
    </div>
    <div class='form-group'>
        <label for='password' class='sr-only'>Password:</label>
        <input type='password' id='password' 
                class='form-control' placeholder='Password'>
    </div>
    <button type="submit" class="btn btn-default">Submit</button>
    <div class="checkbox">
        <label><input type="checkbox"> Remember me</label>
    </div>
</form> 
        </xmp> 
    </div>
</div>


<br /><br />

#### 4. Horizontal Forms

----------------------------------------------------------------------------

<div class="row"> 
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <p>Horizontal forms are similar to inline forms.</p><br><br>
        <form action="#" class="form-horizontal" role="form">
            <div class="form-group">
                <label for="contact-name" class="col-lg-2 control-label">
                    Name</label>
                <div class="col-xs-6">
                    <input type="text" class="form-control" 
                            id="contact-name" placeholder="Name">
                </div>
            </div>
            <div class="form-group">
                <label for="contact-email" class="col-lg-2 control-label">
                    Email</label>
                <div class="col-xs-6">
                    <input type="email" class="form-control" 
                            id="contact-email" placeholder="Email Address">
                </div>
            </div>
            <div class="form-group">
                <label for="contact-message" class="col-lg-2 control-label">
                    Message</label>
                <div class="col-xs-6">
                    <textarea name="contact-message" id="contact-message" 
                            class="form-control" cols="20" rows="10" 
                            placeholder="Message"></textarea>
                </div>
            </div>
        </form>
    </div>
</div>

    <form action="#" class="form-horizontal" role="form">
        
        <div class="form-group">
            <label for="contact-name" class="col-lg-2 control-label">
                Name</label>
            <div class="col-xs-8">
                <input type="text" class="form-control" 
                        id="contact-name" placeholder="Name">
            </div>
        </div>
        
        <div class="form-group">
            <label for="contact-email" class="col-lg-2 control-label">
                Email</label>
            <div class="col-xs-8">
                <input type="email" class="form-control" 
                        id="contact-email" placeholder="Email Address">
            </div>
        </div>

        <div class="form-group">
            <label for="contact-message" class="col-lg-2 control-label">
                Message</label>
            <div class="col-xs-8">
                <textarea name="contact-message" id="contact-message" 
                        class="form-control" cols="20" rows="10" 
                        placeholder="Message"></textarea>
            </div>
        </div>
    </form>         


<br /><br />

#### 5. Form Validation Styling

----------------------------------------------------------------------------


<div class="row"> 
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <p>You can conditionally add some styling after validation fails and the user 
        is redirected. The classes which color the fields are added to the <code>form-group </code>
        divs. We have the classes <code>has-warning has-error</code> and <code>has-success</code></p>
    </div>
</div>
<div class="row">
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br><br>
        <form role='form'>
            <div class="form-group has-warning">
                <input class="form-control" type='text' id='elem-1' placeholder='has-warning'>
            </div>
            <div class="form-group has-error">
                <input class="form-control" type='text' id='elem-2' placeholder='has-warning'>
            </div>
            <div class="form-group has-success">
                <input class="form-control" type='text' id='elem-3' placeholder='has-success'>
            </div>
        </form>
    </div>
    <div class="col-xs-12 col-sm-11 col-sm-offset-1">
<xmp>
<form role='form'>
    <div class="form-group has-warning">
        <input class="form-control" type='text' id='elem-1' placeholder='has-warning'>
    </div>
    <div class="form-group has-error">
        <input class="form-control" type='text' id='elem-2' placeholder='has-warning'>
    </div>
    <div class="form-group has-success">
        <input class="form-control" type='text' id='elem-3' placeholder='has-success'>
    </div>
</form>         
</xmp>
    </div>
</div>
<div class="row"> 
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <p>If you want to do the same for the labels, add the class <code>control-label</code>.</p>
        <br><br>
    </div>
</div>
<div class="row">
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <form role='form'>
            <div class="form-group has-warning">
                <label for='elem-1' class='control-label'>control-label</label>
                <input class="form-control" type='text' id='elem-1' placeholder='has-warning'>
            </div>
            <label for='elem-2' class='control-label'>control-label</label>
            <div class="form-group has-error">
                <input class="form-control" type='text' id='elem-2' placeholder='has-warning'>
            </div>
            <label for='elem-3' class='control-label'>control-label</label>
            <div class="form-group has-success">
                <input class="form-control" type='text' id='elem-3' placeholder='has-success'>
            </div>
        </form>
    </div>
</div>

    <form role='form'>
        <div class="form-group has-warning">
            <input class="form-control" type='text' id='elem-1' placeholder='has-warning'>
        </div>
        <div class="form-group has-error">
            <input class="form-control" type='text' id='elem-2' placeholder='has-warning'>
        </div>
        <div class="form-group has-success">
            <input class="form-control" type='text' id='elem-3' placeholder='has-success'>
        </div>
    </form>         


<div class="row">
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <p>You can additionally add Glyphicons for these three statuses. Each form 
        will need the class of <code>has-feedback</code> along with the 
        <code>has-warning</code> we needed 
        for the colors. A span is added to each form element with the classes 
        <code> glyphicon glyphicon-XYZ form-control form-control-feedback</code>. Shortcuts 
        for these spans in Sublime Text are given as labels below:</p><br><br>
    </div><div class='col-xs-3'></div>
</div>
<div class="row">
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <form role='form'>
            <div class="form-group has-warning has-feedback">
                <label for='elem-1' class='control-label'>
                    span.glyphicon.glyphicon-warning-sign.form-control-feedback</label>
                <input class="form-control" type='text' id='elem-1'>
                <span class="glyphicon glyphicon-warning-sign form-control-feedback"></span>
            </div>
            <div class="form-group has-error has-feedback">
                <label for='elem-2' class='control-label'>
                    span.glyphicon.glyphicon-remove.form-control-feedback</label>
                <input class="form-control" type='text' id='elem-2'>
                <span class="glyphicon glyphicon-remove form-control-feedback"></span>
            </div>
            <div class="form-group has-success has-feedback">
                <label for='elem-3' class='control-label'>
                    span.glyphicon.glyphicon-success.form-control-feedback</label>
                <input class="form-control" type='text' id='elem-3'>
                <span class="glyphicon glyphicon-ok form-control-feedback"></span>
            </div>
        </form>
    </div>
</div>

    <form role='form'>
        <div class="form-group has-warning has-feedback">
            <input class="form-control" type='text' id='elem-1'>
            <span class="glyphicon glyphicon-warning-sign 
                form-control-feedback"></span>
        </div>
        <div class="form-group has-error has-feedback">
            <input class="form-control" type='text' id='elem-2'> 
            <span class="glyphicon glyphicon-remove 
                form-control-feedback"></span>
        </div>
        <div class="form-group has-success has-feedback">
            <input class="form-control" type='text' id='elem-3'>
            <span class="glyphicon glyphicon-ok 
                form-control-feedback"></span>
        </div>
    </form>     


<br /><br />

#### 6. Different Sizes

----------------------------------------------------------------------------

<div class="row"> 
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br>
        <p>You can also control the size of each input element with the class names 
        similar to those for columns, only without xs. </p>
    </div>
</div>
<div class="row"> 
    <div class="col-xs-12 col-sm-11 col-sm-offset-1"><br><br>
        <form role='form'>
            <div class="form-group">
                <input class="form-control input-sm" type='text' id='elem-1' placeholder='input-sm'>
            </div>
            <div class="form-group">
                <input class="form-control input-md" type='text' id='elem-2' placeholder='input-md'>
            </div>
            <div class="form-group">
                <input class="form-control input-lg" type='text' id='elem-3' placeholder='input-lg'>
            </div>
        </form>
    </div>
</div>
<div class="row"> 
    <div class="col-xs-12 col-sm-11 col-sm-offset-1">
        <xmp>
<form role='form'>
    <div class="form-group">
        <input class="form-control input-sm" type='text' id='elem-1' placeholder='input-sm'>
    </div>
    <div class="form-group">
        <input class="form-control input-md" type='text' id='elem-2' placeholder='input-md'>
    </div>
    <div class="form-group">
        <input class="form-control input-lg" type='text' id='elem-3' placeholder='input-lg'>
    </div>
</form>
        </xmp> 
    </div>
</div>
<div class="row"> 
    <div class="col-xs-12 col-sm-101col-sm-offset-1"><br>
        <p>Normally form fields span the full width of the parent container. The  
        reason you are seeing varying widths thought this demonstration is because 
        they are all wrapped within Boostrap col classes, as is customary.</p>
    </div>
</div>







<div class="section jump" id='Dropdowns'><!--#Dropdowns--></div> 

--------------------------------------------------------------------------------

## DROPDOWN MENUS

--------------------------------------------------------------------------------

<div class="row">
	<div class="col-md-9 col-md-offset-1">  
		<p>Dropdown menus are just like buttons but they have the added class of 
		<code>btn-toggle</code> and some extra attributes. Also note that the entire button  
		element is wraped in a div with <code>class='dropdown'</code>. The additional attributes
		in the button element are an <code>id="dd-menu"</code> and an attribute called 
		<code>data-toggle="dropdown"</code>.<br><br>
		Inside the button element you can add a span with the class <code>caret</code> to give it 
		the little dropdown indicating triangle. </p>
	</div>
</div><br>

<div class="row">
	<div class="col-md-1"> <br><br>
		<div class="dropdown">
			<button class='btn btn-default dropdown-toggle' type='button'>
				Dropdown <span class='caret'></span>
			</button>
		</div>  
	</div>
	<div class="col-md-10 col-md-offset-1"> 
		<xmp>
<div class="dropdown">
	<button class='btn btn-default dropdown-toggle' 
					type='button' data-toggle='dropdown'>
		Dropdown <span class='caret'></span>
	</button>
		<!-- add dropdown options here !-->
</div>
		</xmp>
	</div>
</div>

<div class="row">
	<div class="col-md-9 col-md-offset-1">  
		<br><br>
		<p>To specify the option we see when the dropdown is clicked we use an unordered  
		list with <code>class='dropdown-menu'</code> and <code>role='menu'</code>.Each list item optionally have <code>role='presentation'</code> but you should use it. Inside each 
		li tag you have anchor tags which have <code>role='menuitem'</code> and, in 
		order to prevent access by tabbing, <code>tabindex='-1'</code>.</p>
	</div>
</div>

<div class="row">
	<div class="col-md-1"> <br><br>
		<div class="dropdown">
			<button class='btn btn-primary dropdown-toggle' type='button' data-toggle='dropdown'>
				Dropdown <span class='caret'></span>
			</button>
			<ul class='dropdown-menu' role='menu'>
				<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
				<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
				<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
			</ul>
		</div>  
	</div>
	<div class="col-md-10 col-md-offset-1"> 
		<xmp>
<div class="dropdown">
	<button class='btn btn-default dropdown-toggle' type='button' data-toggle='dropdown'>
		Dropdown <span class='caret'></span>
	</button>
	<ul class='dropdown-menu' role='menu'>
		<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
		<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
		<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
	</ul>
</div> 
		</xmp>
		
	</div>
</div>

<!-- !-->
<div class="row">
	<div class="col-md-9 col-md-offset-1">  
		<br><br>
		<p>Add the <code>class='dropdown-header'</code> to a list item and it can be used as a header 
		atop a group of options. Add <code>class='divider'</code> and you'll get a faint line and 
		some spacing between the items it it placed between. Add the <code>class='disabled'</code>
		to gray out an option. </p>
	</div>
</div>

<div class="row">
	<div class="col-md-1"> <br><br>
		<div class="dropdown">
			<button class='btn btn-success dropdown-toggle' type='button' data-toggle='dropdown'>
				Dropdown <span class='caret'></span>
			</button>
			<ul class='dropdown-menu' role='menu'>
				<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
				<li role='presentation' class='dropdown-header'>Header</li>
				<li role='presentation' class='disabled'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
				<li role='presentation' class='divider'></li>
				<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
			</ul>
		</div>  
	</div>
	<div class="col-md-10 col-md-offset-1"> 
		<xmp>
<div class="dropdown">
	<button class='btn btn-success dropdown-toggle' type='button' data-toggle='dropdown'>
		Dropdown <span class='caret'></span>
	</button>
	<ul class='dropdown-menu' role='menu'>
		<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
		<li role='presentation' class='dropdown-header'>Header</li>
		<li role='presentation' class='disabled'></li>
		<li role='presentation' class='divider'></li>
		<li role='presentation'><a href='#' role='menuitem' tabindex='-1'>link1</a></li>
	</ul>
</div> 
		</xmp>
		
	</div>
</div>


<br /><br /><br />

<div class="section jump" id='Tabs'><!--#Tabs--></div> 

----------------------------------------------------------------------------

## Tabs

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-11 col-xs-offset-1">
		<ul class='nav nav-tabs'>
			<li class='active'><a data-toggle="tab" href="#section-1">Section 1</a></li>
			<li><a data-toggle="tab" href="#section-2">Section 2</a></li>
			<li><a data-toggle="tab" href="#section-3">Section 3</a></li>
		</ul>
		<div class="tab-content">
			<div class="tab-pane fade in active" id="section-1">
				<p>This is section 1 content</p>
			</div>
			<div class="tab-pane fade" id="section-2">
				<p>This is section 2 content</p>
			</div>
			<div class="tab-pane fade" id="section-3">
				<p>This is section 3 content</p>
			</div>
		</div>
	</div>
</div> 


The tabs above were created with the code seen. They are an unordered 
list with the classes `nav` and `nav-tabs`. The list 
items are anchors with the `data-toggle` attribute set to 
`tab` rather than `dropdown` as we saw earlier. By 
the way, if you have Sublime Text keybindings you can generate all of the li 
element by typing `li*3>a[data-toggle='tab'][href='#section-$']{Section $}`
and hitting tab! `class='active'` is added to make the first tab selected by 
default.

	<ul class='nav nav-tabs'>
		<li class='active'>
			<a data-toggle="tab" href="#section-1">Section 1</a>
		</li>
		<li><a data-toggle="tab" href="#section-2">Section 2</a></li>
		<li><a data-toggle="tab" href="#section-3">Section 3</a></li>
	</ul>


<p>The content displayed below the tabs by the div you see on the right. Once 
you make the <code>tab-content</code> div you can stub out the other <code>tab-pane</code>
div's in Sublime Text with <code>.tab-pane#section-$*3>p{This is section $ content}</code> 
and hitting tab. <code>fade</code> was added to all tab-panes and the first one gets 
the classes <code>in</code> and <code>active</code>.<br><br>
If you want the tabs to look more like buttons you simply change <code>nav-tabs</code> to 
<code>nav-pills</code></p>

	
	<div class="tab-content">
		<div class="tab-pane fade in active" id="section-1">
			<p>This is section 1 content</p>
		</div>
		<div class="tab-pane fade" id="section-2">
			<p>This is section 2 content</p>
		</div>
		<div class="tab-pane fade" id="section-3">
			<p>This is section 3 content</p>
		</div>
	</div>


<div class="row">
	<div class="col-xs-6">
		<ul class='nav nav-pills'><br><br>
			<li class='active'><a data-toggle="tab" href="#section-1">Section 1</a></li>
			<li><a data-toggle="tab" href="#section-2">Section 2</a></li>
			<li><a data-toggle="tab" href="#section-3">Section 3</a></li>
		</ul>
	</div>
</div>

<br /><br />

<p>If you want them stacked you simply add the class <code>nav-stacked</code>:</p>


<div class="row">
	<div class="col-xs-6">
		<ul class='nav nav-pills nav-stacked'><br><br>
			<li class='active'><a data-toggle="tab" href="#section-1">Section 1</a></li>
			<li><a data-toggle="tab" href="#section-2">Section 2</a></li>
			<li><a data-toggle="tab" href="#section-3">Section 3</a></li>
		</ul>
	</div>
</div>

<br /><br />

Change <code>nav-stacked</code> to<code>nav-justified</code> and you get this:

<div class="row">
	<div class="col-xs-6">
		<ul class='nav nav-pills nav-justified'><br><br>
			<li class='active'><a data-toggle="tab" href="#section-1">Section 1</a></li>
			<li><a data-toggle="tab" href="#section-2">Section 2</a></li>
			<li><a data-toggle="tab" href="#section-3">Section 3</a></li>
		</ul>
	</div>
</div>

<br /><br />

On screen widths smaller than 768px, `nav-justified` will become `nav-stacked`.






<div class="section jump" id='Navbars'><!--#Navbars--></div> 

--------------------------------------------------------------------------------

## NAVBARS

--------------------------------------------------------------------------------


<br /><br />

#### 1. The nav element

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-12">
		<nav class="navbar navbar-default" role="navigation">
		</nav>
	</div>
</div>

The bare minimum to make a navbar as seen above is this code:

<br />

	<nav class="navbar navbar-default" role="navigation">
	</nav>



<br /><br />

#### 2. Navbar container

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-12">
		<nav class="navbar navbar-default" role="navigation">
			<div class="container">
				<div class="navbar-header">
					<a href='#' class='navbar-brand'>Brand</a>
				</div>
			</div>
		</nav>
	</div>
</div>

Place all of your navbar components inside a div container with 
`class="navbar-header"`. To create a title on the left side create a div and 
inside the div, add an anchor with the `class='navbar-brand'` which is the
term for title or logo for your site. Here is the code for the navbar above.

<br />

	<nav class="navbar navbar-default" role="navigation">
		<div class="container">
			<div class="navbar-header">
				<a href='#' class='navbar-brand'>Brand</a>
			</div>
		</div>
	</nav>



<br /><br />

#### 3. The Three Lined Button

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-12">
		<nav class="navbar navbar-default" role="navigation">
			<div class="container">
				<div class="navbar-header">
					<button type='button' class='navbar-toggle' data-toggle='collapse' 
													data-target='#example-nav-collapse'>
						<span class='sr-only'>Toggle navigation</span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
					</button>
					<a href='#' class='navbar-brand'>Brand</a>
				</div>
			</div>
		</nav>
	</div>
</div>

<br />

For a button that will appear in response to a smaller screen we will create 
a button with the `class='navbar-toggle'` and `data-toggle'collapse'`. Right now 
all we have on our navbar is a title, but once we have items that can't fit 
on smaller screens, they will be added to the dropdown of this button. It
also needs a `data-target` which will match the id of our navbar elements. 
The need for this becomes clear if you have more than one navbar and they 
start showing each other's elements!<br /> 

Let's set that target to `#example-nav-collapse`. The button itself 
is comprised of three horizontal lines. In Sublime Text you can type 
`span.icon-bar*3` and hit tab. If you shrink the window you will see the 
button appear on the right side of the navbar. The span with `class='sr-only'`
is used for accessibility and can only be seen on screen readers. Here is 
all the code:
	

	<nav class="navbar navbar-default" role="navigation">
		<div class="container">
			<div class="navbar-header">
				<button type='button' class='navbar-toggle' data-toggle='collapse' 
												data-target='#example3-nav-collapse'>
					<span class='sr-only'>Toggle navigation</span>
					<span class="icon-bar"></span>
					<span class="icon-bar"></span>
					<span class="icon-bar"></span>
				</button>
				<a href='#' class='navbar-brand'>Brand</a>
			</div>
		</div>
	</nav>



<br /><br />

#### 4. Adding Links:

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-12">
		<nav class="navbar navbar-default" role="navigation">
			<div class="container">
				<div class="navbar-header">
					<button type='button' class='navbar-toggle' data-toggle='collapse' 
													data-target='#example4-nav-collapse'>
						<span class='sr-only'>Toggle navigation</span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
					</button>
					<a href='#' class='navbar-brand'>Brand</a>
				</div>
				<div class="collapse navbar-collapse" id="example4-nav-collapse">
					<ul class='nav navbar-nav'>
						<li class='active'><a>Link 1</a></li>
						<li><a>Link 2</a></li>
					</ul>
				</div>
			</div>
		</nav>
	</div>
</div>

All of what we have now is in the `navbar-header` div. Still inside of the 
container but outside of `navbar-header` we can create the items on the navbar. 
We will create a new div with the same id as the button. It will have the 
classes `collapse` and `navbar-collapse` so it moved to the button when the 
screen collapses. In Sublime Text type 
`.collapse.navbar-collapse#example-nav-collapse` and hit tab. Inside that 
you can put anything you want. You can put links, dropdown menus, forms etc. 
Above, we created a `ul` with classes `nav` and `navbar-nav` with two links and
made the first one be active.

<br />

	<nav class="navbar navbar-default" role="navigation">
		...
			<div class="collapse navbar-collapse" id="example-nav-collapse">
				<ul class='nav navbar-nav'>
					<li class='active'><a>Link 1</a></li>
					<li><a>Link 2</a></li>
				</ul>
			</div>
		</div>
	</nav>


<br /><br />

#### 5. A Search Box

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-12">
		<nav class="navbar navbar-default" role="navigation">
			<div class="container">
				<div class="navbar-header">
					<button type='button' class='navbar-toggle' data-toggle='collapse' 
													data-target='#example5-nav-collapse'>
						<span class='sr-only'>Toggle navigation</span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
					</button>
					<a href='#' class='navbar-brand'>Brand</a>
				</div>
				<div class="collapse navbar-collapse" id="example5-nav-collapse">
					<ul class='nav navbar-nav'>
						<li class='active'><a>Link 1</a></li>
						<li><a>Link 2</a></li>
					</ul>
					
					<form role='' class="navbar-form navbar-left role='search">
						<div class="form-group">
							<input type='text' class='form-control' placeholder='Search'>
						</div>
						<button type='submit' class='btn btn-default'>Submit</button>
					</form>
				</div>
			</div>
		</nav>
	</div>
</div>



To put a search box we will use a form. `form.navbar-form.navbar-left` and 
hit tab add a role='search' and create a div inside it with the class 
`form-group` just as we do with forms. The rest is as expected with forms. 
You can change the form class to `navbar-right` if you want it on the right. 
<br /><br />
Now is a good time to see the collapse in action. Make the screen smaller 
and you will see everything but the title vanish and the button appear. 
Click on the button and there they are!

<br />

	<nav class="navbar navbar-default" role="navigation">
		...
			<div class="collapse navbar-collapse" id="example-nav-collapse">
				<ul class='nav navbar-nav'>
					<li class='active'><a>Link 1</a></li>
					<li><a>Link 2</a></li>
				</ul>
				
				<form role='' class="navbar-form navbar-left role='search">
					<div class="form-group">
						<input type='text' class='form-control' placeholder='Search'>
					</div>
					<button type='submit' class='btn btn-default'>Submit</button>
				</form>
			</div>
		</div>
	</nav>



<br /><br />

#### 6. Adding Other Elements

----------------------------------------------------------------------------

<div class="row">
	<div class="col-xs-12">
		<nav class="navbar navbar-default" role="navigation">
			<div class="navbar-header">
				<button type='button' class='navbar-toggle' data-toggle='collapse' 
												data-target='#example6-nav-collapse'>
					<span class='sr-only'>Toggle navigation</span>
					<span class="icon-bar"></span>
					<span class="icon-bar"></span>
					<span class="icon-bar"></span>
				</button>
				<a href='#' class='navbar-brand'>Brand</a>
			</div>
			<div class="collapse navbar-collapse" id="example6-nav-collapse">
				<ul class='nav navbar-nav'>
					<li class='active'><a>Link 1</a></li>
					<li><a>Link 2</a></li>
				</ul>
				<a href='#' class="btn btn-default navbar-btn">Button</a>
				<p class="navbar-text">Hello!</p>
				<form role='' class="navbar-form navbar-right role='search">
					<div class="form-group">
						<input type='text' class='form-control' placeholder='Search'>
					</div>
					<button type='submit' class='btn btn-default'>Submit</button>
				</form>
			</div>
		</nav>
	</div>
</div>

<br />

The seach, or any element, can be moved to the right with the `navbar-right` class. 
Adding other elements can break the style unless you add the right bootstrap 
classes. 

<br />

	<nav class="navbar navbar-default" role="navigation">
			...
				<a href='#' class="btn btn-default navbar-btn">Button</a>
				<p class="navbar-text">Hello!</p>
			...
	</nav>



<br /><br />

#### 7. Navbar Options

----------------------------------------------------------------------------

Adding the class `navbar-fixed-top` places it on the top of the page no 
matter how far down the user has scrolled. Likewise you can use 
`navbar-fixed-bottom`. If you want inverted colors use `navbar-inverse` 
instead of `navbar-default`.



<br /><br />

#### 8. Scroll Spy

----------------------------------------------------------------------------

Rather that breaking up your site into many pages you can have all of 
the content on one page with navigation to each section via a navbar, for 
example. The navbar can contain href links to id's placed in tags throughout 
your page. <br /><br />
If the navbar is fixed at the top or botton it would be nice to 
have it display the current section being viewed. This is possible 
by adding some bootstrap attributes to the body of the page. We are 
tracking scrolling so we add `data-spy='scroll'`. The navagation element was 
given an id and we will target that by adding `data-target='#main-navbar'`
(in the case of the navbar having `id='main-navbar'`). This is all you need 
to do!<br /><br />
An example is given below:

	<nav class="navbar navbar-inverse navbar-fixed-bottom" id="demo-navbar" role="navigation">
		<div class="container">
			<div class="navbar-header">
				<button class="navbar-toggle" type="button" 
						data-toggle="collapse" data-target'#navbar-collapse'>
					<span class="sr-only">Toggle navigation</span>
					<span class="icon-bar"></span>
					<span class="icon-bar"></span>
					<span class="icon-bar"></span>
				</button>
			</div>
			<div class="collapse navbar-collapse" id="navbar-collapse">
				<ul class="nav navbar-nav">
					<li><a href="#section1">section1</a></li>
					<li><a href="#section2">section2</a></li>
					<li><a href="#section3">section3</a></li>
					<li><a href="#section4">section4</a></li>
				</ul>
			</div>
		</div>
	</nav>





<div class="section jump" id='ListGroups'><!--#ListGroups--></div> 

--------------------------------------------------------------------------------

## LIST GROUPS

--------------------------------------------------------------------------------


<br /><br />

#### 1. As Unordered Lists

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-sm-5 col-xs-offset-1">
		<br><p>List groups allow for way to style HTML lists with bootstrap. It is list 
		group could be an unordered list with the class <code>list-group</code> where each item 
		has the class <code>list-group-item</code>. In Sublime Text type 
		<code>ul.list-group>li.list-group-item{Item $}*4</code> and hit tab.</p><br>
	</div>
	<div class="col-sm-5 col-xs-offset-1 col-sm-offset-0 black-text">
		<br>
		<ul class="list-group">
			<li class="list-group-item">Item 1</li>
			<li class="list-group-item">Item 2</li>
			<li class="list-group-item">Item 3</li>
			<li class="list-group-item">Item 4</li>
		</ul>
	</div>
</div>
	
	<ul class="list-group">
		<li class="list-group-item">Item 1</li>
		<li class="list-group-item">Item 2</li>
		<li class="list-group-item">Item 3</li>
		<li class="list-group-item">Item 4</li>
	</ul>


<br /><br />

#### 2. As Divs Containing Links

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-sm-5 col-xs-offset-1">
		<br><p>You can also use a div with anchor tags instead of <code>ul</code>
		with <code>li</code>, respectively. Make one <code>list-group-item</code> 
		active by adding the class <code>active</code>. Bootstrap 
		colors can be added with the class <code>list-group-item-XYZ</code> where XYZ could be 
		<code>success info warning</code> or <code>danger</code>.</p>
		<br>
	</div>
	<div class="col-sm-5 col-xs-offset-1 col-sm-offset-0 black-text">
		<br>
		<div class='list-group'>
			<a class="list-group-item list-group-item-success active">Item 1</a>
			<a class="list-group-item list-group-item-info">Item 2</a>
			<a class="list-group-item list-group-item-warning">Item 3</a>
			<a class="list-group-item list-group-item-danger">Item 4</a>
		</div>
	</div>
</div>

	<div class='list-group'>
		<a class="list-group-item list-group-item-success active">Item 1</a>
		<a class="list-group-item list-group-item-info">Item 2</a>
		<a class="list-group-item list-group-item-warning">Item 3</a>
		<a class="list-group-item list-group-item-danger">Item 4</a>
	</div>

<br /><br />

#### 3. With Custom Content

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-md-5 col-xs-offset-1">
		<br><br><p>You aren't limited to just li's and a' in a list group. You can have 
		headers with the class l<code>ist-group-item-heading</code> and text with the class 
		<code>list-group-item-heading</code>:</p>
	</div>
	<div class="col-xs-11 col-md-5 col-xs-offset-1 col-md-offset-0 black-text">
		<div class='list-group'>
			<a class="list-group-item list-group-item-success active">
				<h4 class='list-group-item-heading'>list-group-item-heading</h4>
				<p class='list-group-item-text'>list-group-item-text</p>
			</a>
			<a class="list-group-item list-group-item-info ">
				<h4 class='list-group-item-heading'>list-group-item-heading</h4>
				<p class='list-group-item-text'>list-group-item-text</p>
			</a>
			<a class="list-group-item list-group-item-danger ">
				<h4 class='list-group-item-heading'>list-group-item-heading</h4>
				<p class='list-group-item-text'>list-group-item-text</p>
			</a>
		</div>
	</div>
</div>

	<div class='list-group'>
		<a class="list-group-item list-group-item-success active">
			<h4 class='list-group-item-heading'>list-group-item-heading</h4>
			<p class='list-group-item-text'>list-group-item-text</p>
		</a>
		<a class="list-group-item list-group-item-info ">
			<h4 class='list-group-item-heading'>list-group-item-heading</h4>
			<p class='list-group-item-text'>list-group-item-text</p>
		</a>
		<a class="list-group-item list-group-item-danger ">
			<h4 class='list-group-item-heading'>list-group-item-heading</h4>
			<p class='list-group-item-text'>list-group-item-text</p>
		</a>
	</div>

 





<div class="section jump" id='Panels'><!--#Panels--></div> 

--------------------------------------------------------------------------------

## PANELS

--------------------------------------------------------------------------------

<br /><br />

#### 1. Panel Basics

----------------------------------------------------------------------------


Panels allow you to organize your content into visible boxes. The four 
most important divs contain the classes `panel panel-default`, 
`panel-heading`, `panel-body` and `panel-footer`. The div with 
`class='panel panel-default` contains the other three divs. 

<div class='row'>
	<div class="col-xs-10 col-sm-8 col-md-6 col-xs-offset-1 black-text">
		<br>
		<div class="panel panel-default">
			<div class="panel-heading">Heading</div>
			<div class="panel-body">Body</div>
			<div class="panel-footer">Footer</div>
		</div>
	</div>
</div>


	<div class="panel panel-default">
		<div class="panel-heading">Heading</div>
		<div class="panel-body">Body</div>
		<div class="panel-footer">Footer</div>
	</div>



<br /><br />

#### 2. Titles and Footers

----------------------------------------------------------------------------


To change the color scheme of the entire panel you can add the class 
`panel-XYZ` where XYZ could be `primary`, `success`, `info`, `warning` or `danger`. 
If you want more emphasis on the heading you can wrap it in a header
tag with the class `panel-title`.

<div class='row'>
	<div class="col-xs-10 col-sm-8 col-md-6 col-xs-offset-1 black-text">
		<br>
		<div class="panel panel-default panel-info">
			<div class="panel-heading">
				<h4 class='panel-title'>Heading</h4>
			</div>
			<div class="panel-body">Body</div>
			<div class="panel-footer">Footer</div>
		</div>
	</div>
</div>


	<div class="panel panel-default panel-info">
		<div class="panel-heading">
			<h4 class='panel-title'>Heading</h4>
		</div>
		<div class="panel-body">Body</div>
		<div class="panel-footer">Footer</div>
	</div>



<br /><br />

#### 3. Panels with Tables

----------------------------------------------------------------------------


Bootstrap Panels integrate very well with HTML tables. Add the bootstrap 
class `table` to an HTML table tag and put it anywhere inside the panel's 
parent div.

<div class='row'>
	<div class="col-xs-10 col-sm-8 col-md-6 col-xs-offset-1 black-text">
		<br><br>
		<div class="panel panel-default panel-info">
			<div class="panel-heading">
				<h4 class='panel-title'>Heading</h4>
			</div>
			<div class="panel-body">Body</div>
			<table class="table">
				<tr>
					<th>Heading 1</th>
					<th>Heading 2</th>
					<th>Heading 3</th>
				</tr>
				<tr>
					<td>Cell 1</td>
					<td>Cell 2</td>
					<td>Cell 3</td>
				</tr>
				<tr>
					<td>Cell 1</td>
					<td>Cell 2</td>
					<td>Cell 3</td>
				</tr>
			</table>
			<div class="panel-footer">Footer</div>
		</div>
	</div>
</div>

	<div class="panel panel-default panel-info">
		...
		<table class="table">
			<tr>
				<th>Heading 1</th>
				<th>Heading 2</th>
				<th>Heading 3</th>
			</tr>
			<tr>
				<td>Cell 1</td>
				<td>Cell 2</td>
				<td>Cell 3</td>
			</tr>
			<tr>
				<td>Cell 1</td>
				<td>Cell 2</td>
				<td>Cell 3</td>
			</tr>
		</table>
		...
	</div>


<br /><br />

#### 4. Panels with List Groups

----------------------------------------------------------------------------


Bootstrap Panels also integrate very well with Bootstrap List Groups. 
Just define a list group exactly as you normally would and place it 
anywhere inside the panel's parent div.

<div class='row'>
	<div class="col-xs-10 col-sm-8 col-md-6 col-xs-offset-1 black-text">
		<br>
		<div class="panel panel-default panel-info">
			<div class="panel-heading">
				<h4 class='panel-title'>Heading</h4>
			</div>
			<div class="panel-body">Body</div>
			<ul class="list-group">
				<li class="list-group-item">List Item 1</li>
				<li class="list-group-item">List Item 2</li>
				<li class="list-group-item">List Item 3</li>
				<li class="list-group-item">List Item 4</li>
			</ul>
			<div class="panel-footer">Footer</div>
		</div>
	</div>
</div>

			
	<div class="panel panel-default panel-info">
		...
		<ul class="list-group">
			<li class="list-group-item">List Item 1</li>
			<li class="list-group-item">List Item 2</li>
			<li class="list-group-item">List Item 3</li>
			<li class="list-group-item">List Item 4</li>
		</ul>
		...
	</div>


<br /><br />

#### 5. Panel Groups

----------------------------------------------------------------------------

You can collapse and expand portions of the page like an accordion using 
the `panel-collapse class`. Each of these portions will be a panel within a 
panel group. This is the first step to making a `panel-collapse`. We assigned 
an `id` to the group, which will be needed later.

<div class='row'>
	<div class="col-xs-10 col-sm-8 col-md-6 col-xs-offset-1 black-text">
		<br><br><br>
		<div class="panel-group">
			<div class="panel panel-default">
				<div class="panel-heading">
					<h4 class='panel-title'>Heading 1</h4>
				</div>
				<div class="panel-body">Body 1</div>
			</div>
			<div class="panel panel-default">
				<div class="panel-heading">
					<h4 class='panel-title'>Heading 2</h4>
				</div>
				<div class="panel-body">Body 2</div>
			</div>
			<div class="panel panel-default">
				<div class="panel-heading">
					<h4 class='panel-title'>Heading 2</h4>
				</div>
				<div class="panel-body">Body 2</div>
			</div>
		</div>
	</div>
</div>

	<div class="panel-group" id="accordion">
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class='panel-title'>Heading 1</h4>
			</div>
			<div class="panel-body">Body 1</div>
		</div>
		
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class='panel-title'>Heading 2</h4>
			</div>
			<div class="panel-body">Body 2</div>
		</div>
		
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class='panel-title'>Heading 2</h4>
			</div>
			<div class="panel-body">Body 2</div>
		</div>
	</div>


<br /><br />

#### 6. Panel Collapse

----------------------------------------------------------------------------


Now that we have the group set we can set it up so that only one panel is 
showing at a time. Expanding one collapses the others. First we change the 
contents of the titles to that they are links to the body. We'll wrap each 
body in a div with an id that matches the link. In addition to the href 
being the id, each anchor also needs `data-toggle="collapse"` and 
`data-parent="#accordion'`. As for the div's around each body, in addition 
their id's they also need `class="panel-collapse collapse"`. Note that the 
first panel's body has the additional `class='` ... `in'`. This makes it be 
expanded right from the start.

<div class='row'>
	<div class="col-xs-10 col-sm-8 col-md-6 col-xs-offset-1 black-text">
		<br><br><br>
	
		<div class="panel-group" id="accordion">
			<div class="panel panel-default">
				<div class="panel-heading">
					<h4 class="panel-title">
						<a href="#body-1" data-toggle="collapse" 
							data-parent="#accordion">Heading 1</a></h4>
				</div>
				<div class="panel-collapse collapse in" id="body-1">
					<div class="panel-body">Body 1</div>
				</div>
			</div>
			<div class="panel panel-default">
				<div class="panel-heading">
					<h4 class="panel-title">
						<a href="#body-2" data-toggle="collapse" 
							data-parent="#accordion">Heading 2</a></h4>
				</div>
				<div class="panel-collapse collapse" id="body-2">
					<div class="panel-body">Body 2</div>
				</div>
			</div>
			<div class="panel panel-default">
				<div class="panel-heading">
					<h4 class="panel-title">
						<a href="#body-3" data-toggle="collapse" 
							data-parent="#accordion">Heading 3</a></h4>
				</div>
				<div class="panel-collapse collapse" id="body-3">
					<div class="panel-body">Body 3</div>
				</div>
			</div>
		</div>
	</div>
</div>

	<div class="panel-group" id="accordion">
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class="panel-title">
					<a href="#body-1" data-toggle="collapse" 
						data-parent="#accordion">Heading 1</a></h4>
			</div>
			<div class="panel-collapse collapse in" id="body-1">
				<div class="panel-body">Body 1</div>
			</div>
		</div>
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class="panel-title">
					<a href="#body-2" data-toggle="collapse" 
						data-parent="#accordion">Heading 2</a></h4>
			</div>
			<div class="panel-collapse collapse" id="body-2">
				<div class="panel-body">Body 2</div>
			</div>
		</div>
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class="panel-title">
					<a href="#body-3" data-toggle="collapse" 
						data-parent="#accordion">Heading 3</a></h4>
			</div>
			<div class="panel-collapse collapse" id="body-3">
				<div class="panel-body">Body 3</div>
			</div>
		</div>
	</div>






<div class="section jump" id='Images'><!--#Images--></div> 

--------------------------------------------------------------------------------

## IMAGES CAROUSELS

--------------------------------------------------------------------------------

<br /><br />

#### 1. Basic Carousels

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-xs-11 col-xs-offset-1 col-md-5 ">
		<p>Bootstrap carousels are picture slides. They sit inside a div with the 
		classes <code>carousel</code> and <code>slide</code>. Set any id for this div 
		and set an attribute called <code>data-ride</code> to <code>carousel</code>. 
		Inside this div you will have an ordered list 
		which keeps track of all the pictures and another div containing the pictures 
		which has a class of <code>carousel-inner</code>. <br><br> 
	</div>
	<div class="col-xs-11 col-xs-offset-1 col-md-6 col-md-offset-0">
		<div class="carousel slide" id="img-slides" data-ride="carousel">
			<ol class="carousel-indicators">
				<li data-target="#img-slides" data-slide-to="0" class='active'></li>
				<li data-target="#img-slides" data-slide-to="1"></li>
				<li data-target="#img-slides" data-slide-to="2"></li>
			</ol>
		
			<div class="carousel-inner">
				<div class="item active">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat1.jpg_zpsxy3fcfoq.png" alt="Slide">
				</div>
				<div class="item">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat2_zpskrcaeag7.jpg" alt="Slide">
				</div>
				<div class="item">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat3.jpg_zpslfcmjatu.png" alt="Slide">
				</div>
			</div>
		</div>
	</div>	
</div>

The ordered list has a class of 
<code>carousel-indicators</code>. Each li has <code>data-target</code> set to 
the id with a <code>#</code> added 
before. They also each have an attribute <code>data-slide-to</code> which is set to an 
integer index starting at zero. The first appearing picture should have 
<code>class='active' added</code>.<br><br>
As for the <code>carousel-inner</code> div, each img element is wrapped in a div with 
<code>class='item'</code> and the added class <code>active</code> for the 
first appearing picture.</p>




	<div class="carousel slide" id="img-slides" data-ride="carousel">
		<ol class="carousel-indicators">
			<li data-target="#img-slides" data-slide-to="0" class='active'></li>
			<li data-target="#img-slides" data-slide-to="1"></li>
			<li data-target="#img-slides" data-slide-to="2"></li>
		</ol>

		<div class="carousel-inner">
			<div class="item active">
				<img src="/assets/cat1.jpg" alt="Slide">
			</div>
			<div class="item">
				<img src="/assets/cat2.jpg" alt="Slide">
			</div>
			<div class="item">
				<img src="/assets/cat3.jpg" alt="Slide">
			</div>
		</div>
	</div>


<br /><br />

#### 2. Side Arrows

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-xs-11 col-xs-offset-1 col-md-5 ">
		<p>If you want arrows on the left and right sides you just need to add a 
		little bit of code as the last thing in the <code>carousel slide</code> div. It will 
		be two anchors with href set to the id of the carousel with a <code>#</code>sign before. 
		One will have the class of <code>left carousel-control</code> and 
		<code>data-slide='prev'</code>
		and the other will have the class of <code>right carousel-control</code> and 
		<code>data-slide='prev'</code>. Inside each anchor tag you can place a a span with a 
		glyphicon.</p>
	</div>
	<div class="col-xs-11 col-xs-offset-1 col-md-6 col-md-offset-0">
		<div class="carousel slide" id="img-slides2" data-ride="carousel">
			<ol class="carousel-indicators">
				<li data-target="#img-slides2" data-slide-to="0" class='active'></li>
				<li data-target="#img-slides2" data-slide-to="1"></li>
				<li data-target="#img-slides2" data-slide-to="2"></li>
			</ol>
			<div class="carousel-inner">
				<div class="item active">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat1.jpg_zpsxy3fcfoq.png" alt="Slide">
				</div>
				<div class="item">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat2_zpskrcaeag7.jpg" alt="Slide">
				</div>
				<div class="item">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat3.jpg_zpslfcmjatu.png" alt="Slide">
				</div>
			</div>
			<a href='#img-slides2' class="left carousel-control" data-slide='prev'>
				<span class="glyphicon glyphicon-chevron-left"></span>
			</a>
			<a href='#img-slides2' class="right carousel-control" data-slide='next'>
				<span class="glyphicon glyphicon-chevron-right"></span>
			</a>
		</div>
	</div>	
</div>

<br /><br />

	<div class="carousel slide" id="img-slides" data-ride="carousel">
		...
		<a href='#img-slides2' class="left carousel-control" data-slide='prev'>
			<span class="glyphicon glyphicon-chevron-left"></span>
		</a>
		<a href='#img-slides2' class="right carousel-control" data-slide='next'>
			<span class="glyphicon glyphicon-chevron-right"></span>
		</a>
	</div>

<br /><br />

#### 3. Captions

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-xs-11 col-xs-offset-1 col-md-5 ">
		<p>If you want a caption at the bottom of each picture you can add them 
		with a div with the class of <code>carousel-caption</code>. They go in the same item div
		you put the img elements in. You can add things like headings or paragraphs here. 
		</p>
	</div>
	<div class="col-xs-11 col-xs-offset-1 col-md-6 col-md-offset-0">
		<div class="carousel slide" id="img-slides3" data-ride="carousel">
			<ol class="carousel-indicators">
				<li data-target="#img-slides3" data-slide-to="0" class='active'></li>
				<li data-target="#img-slides3" data-slide-to="1"></li>
				<li data-target="#img-slides3" data-slide-to="2"></li>
			</ol>
			<div class="carousel-inner">
				<div class="item active">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat1.jpg_zpsxy3fcfoq.png" alt="Slide">
					<div class="carousel-caption">
						<h3>Heading</h3>
						<p>some info about this picture</p>
					</div>
				</div>
				<div class="item">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat2_zpskrcaeag7.jpg" alt="Slide">
					<div class="carousel-caption">
						<h3>Heading</h3>
						<p>some info about this picture</p>
					</div>
				</div>
				<div class="item">
					<img src="http://i1377.photobucket.com/albums/ah75/Jeffrey_Russ/cat3.jpg_zpslfcmjatu.png" alt="Slide">
					<div class="carousel-caption">
						<h3>Heading</h3>
						<p>some info about this picture</p>
					</div>
				</div>
			</div>
			<a href='#img-slides3' class="left carousel-control" data-slide='prev'>
				<span class="glyphicon glyphicon-chevron-left"></span>
			</a>
			<a href='#img-slides3' class="right carousel-control" data-slide='next'>
				<span class="glyphicon glyphicon-chevron-right"></span>
			</a>
		</div>
	</div>
</div>

<br /><br />

	<div class="carousel slide" id="img-slides3" data-ride="carousel">
		...
		<div class="carousel-inner">
			<div class="item active">
				<img src="/assets/cat1.jpg" alt="Slide">
				<div class="carousel-caption">
					<h3>Heading</h3>
					<p>some info about this picture</p>
				</div>
			</div>
			...
	</div>


<br /><br />

#### 4. Responsive Images

----------------------------------------------------------------------------

<div class='row'>
	<div class="col-xs-12 col-sm-11 col-xs-offset-1">
		<p>The bootstrap class <code>img-responsive</code> will apply max width 100% and and height 
		auto to an img element's image. This makes it resize according to it's parent. <p>
	</div>
</div>




<div class="section jump" id='Modals'><!--#Modals--></div> 

--------------------------------------------------------------------------------

## MODAL WINDOWS

----------------------------------------------------------------------------

<br /><br />

#### 1. The Parent Divs

----------------------------------------------------------------------------

Modal Windows allow windows to pop up over the screen temporarily, usually 
for the user to make a selection. Three divs are used to contain the 
content of your modal window, the outermost with the class modal, the next 
with the class `modal-dialog` and the innermost with the class `modal-content`.
<br />
Additionally, the outermost div needs an id, a `tabindex='-1'` to block use 
of the tab button and `role='dialog'`. It's quite a bit but a good way to 
stub it out it in Sublime Text: `.modal#modal-1>.modal-dialog>.modal-content` 
and hit tab. then just add the `tabindex` and `role`. <br /><br />
Inside the innermost div we will have three divs with the classes 
`modal-header`, `modal-body` and `modal-footer`. The body will be the content.

	<div class="modal" id="modal-1" tabindex='-1' role='dialog '>
		<div class="modal-dialog">
			<div class="modal-content">
				
				<div class="modal-header"></div>
				<div class="modal-body">Content</div>
				<div class="modal-footer"></div>
				
			</div>
		</div>
	</div>


<br /><br />

#### 2. The Header

----------------------------------------------------------------------------

The header usually contains the close button and the title for the content.
The button needs the class `close` and `type='button'` and an attribute called 
`data-dismiss` set to `modal`. The content of the button is the red x symbol. 
<br><br>
For the title we will use an `h4` tag with the class `modal-title`

	
	<div class="modal" id="modal-1" tabindex='-1' role='dialog'>
		<div class="modal-dialog">
			<div class="modal-content">
				
				<div class="modal-header">
					<button type="button" class="close" data-dismiss='modal'>
						&times;</button>
					<h4 class="modal-title">modal-title</h4>
				</div>
				<div class="modal-body">Content</div>
				<div class="modal-footer"></div>
				
			</div>
		</div>
	</div>


<br /><br />

#### 3. An Open Button

----------------------------------------------------------------------------


The open button is placed outside of the parent modal div, usually before 
everything. It has the usual class of `btn btn-WHATEVER` and `type='button`. 
Additionally, it needs `data-toggle='modal'` and the attribute `data-target`
set to the id of the modal class, with a `#` added before it's name. It 
works now... click and see. 

<div class="row">
	<div class="col-xs-11 col-xs-offset-1">
		<button type='button' class="btn btn-primary" data-toggle='modal' 
				data-target='#modal-1'>It works!</button>
		<div class="modal" id="modal-1" tabindex='-1' role='dialog '>
			<div class="modal-dialog">
				<div class="modal-content black-text">
					<div class="modal-header">
						<button type="button" class="close" data-dismiss='modal'>
							&times;</button>
						<h4 class="modal-title">modal-title</h4>
					</div>
					<div class="modal-body">Content</div>
					<div class="modal-footer"></div>
				</div>
			</div>
		</div>
	</div>	
</div>

<br />
			
	<button type='button' class="btn btn-primary" data-toggle='modal' 
			data-target='#modal-1'>It works!</button>
			
	<div class="modal" id="modal-1" tabindex='-1' role='dialog '>
		...
	</div>

<br /><br />

#### 4. The Footer

----------------------------------------------------------------------------


The div with `modal-footer` is where you would put your buttons as in the 
case of this modal window being a dialog box. We already have a close 
button as an X in the upper right but now we can make a proper button on 
the bottom, along with a save button, for example.
<br /><br />
The close button is has the same `data-dismiss='modal'` as we have seen 
previously. 

<div class='row'>
	<div class="col-xs-11 col-xs-offset-1"><br>
		<button type='button' class="btn btn-primary" data-toggle='modal' 
				data-target='#modal-2'>w/Footer</button>
		<div class="modal" id="modal-2" tabindex='-1' role='dialog '>
			<div class="modal-dialog">
				<div class="modal-content black-text">
					<div class="modal-header">
						<button type="button" class="close" data-dismiss='modal'>
							&times;</button>
						<h4 class="modal-title">modal-title</h4>
					</div>
					<div class="modal-body">Content</div>
					<div class="modal-footer">
						<a href='#' class="btn btn-default" data-dismiss='modal'>
							Close</a>
						<a href='#' class="btn btn primary">Save</a>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>

<br />

	<div class="modal-footer">
		<a href='#' class="btn btn-default" data-dismiss='modal'>
			Close</a>
		<a href='#' class="btn btn primary">Save</a>
	</div>

<br /><br />

#### 5. Other Options

----------------------------------------------------------------------------

For a fade effect, simply add the class `fade` to the div with `modal`. You 
can use `.modal-lg` along with `.modal-dialog` for a larger window. You can 
use `.modal-sm` along with `.modal-dialog` for a larger window.



<small><hr></small>
<a href='http://www.jeffruss.com' style='color:#FFFFEE'>
<small>    © Copyright 2016 Jeffrey Russ</small><br><br><br>
</a>







