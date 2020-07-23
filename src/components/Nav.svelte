<script>
	export let segment;
</script>

<style>
	nav {
		border-bottom: 1px solid rgba(255,62,0,0.1);
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: right;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
		font-size: 18px;
		font-family: SansPro;
	}
	.logo{
		display: inline-block;
		position: absolute;
		top: 15px;
		
	}
	@media only screen and (max-width: 765px){
	li {
		display: block;
		float:right;
		text-align: center;
		margin-top: 50px;
	}
	}

	@media only screen and (max-width: 493px){
	a{
		font-size: 16px;
	}
}
</style>

<nav>
<div class="logo"><h2>PureSaneo</h2></div>
	<ul>
		
		<li><a aria-current="{segment === 'contact' ? 'page' : undefined}" href="#Fifth_Section">Contact</a></li>
		<li><a aria-current="{segment === 'deal' ? 'page' : undefined}" href="#Third_Section">Get a deal</a></li>
		<li><a aria-current="{segment === 'galery' ? 'page' : undefined}" href="#Second_Section">Gallery</a></li>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href="#First_Section">Why us ?</a></li>
		
		
	</ul>
</nav>
