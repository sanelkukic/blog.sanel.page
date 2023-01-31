Type: Template
Title: No Recents

<!DOCTYPE html>
<html lang="en" prefix="og: https://ogp.me/ns#">
<head>
{feeds}
<title>{weblog-title}{separator}{post-title}</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta property="og:title" content="{weblog-title}"/>
<meta property="og:description" content="{weblog-description}"/>
<meta property="og:url" content="https://blog.sanel.page"/>
<meta property="og:locale" content="en_US"/>
<meta property="og:site_name" content="weblog.lol"/>
<meta property="og:type" content="website"/>
<meta name="theme-color" content="#fabc02" media="(prefers-color-scheme: light)">
<meta name="theme-color" content="#fabc02" media="(prefers-color-scheme: dark)">
<script src="https://js.cache.lol/snowstorm.js"></script>
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-TC25Q5BLWG"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-TC25Q5BLWG');
</script>
<style>
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-lato-regular.css');
@import url('https://static.omg.lol/type/font-lato-bold.css');
@import url('https://static.omg.lol/type/font-lato-italic.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');

:root {
	--foreground: #fff;
	--background: #212121;
	--link: #fabc02;
	--accent: #fabc02;
}

@media (prefers-color-scheme: dark) {
	:root {
		--foreground: #fff;
		--background: #212121;
		--link: #fabc02;
		--accent: #fabc02;
	}
}

* {
	box-sizing: border-box;
}

body {
	font-family: 'Lato', sans-serif;
	font-size: 120%;
	color: var(--foreground);
	background: var(--background);
}

header nav ul {
	list-style-type: none;
	margin: 0;
	padding: 0;
}

header nav li {
	display: inline-block;
}

header nav li a {
	display: block;
	//text-decoration: none;
	margin-right: 1em;
}

h1, h2, h3, h4, h5, h6 {
	font-family: 'VC Honey Deck', serif;
	margin: 1rem 0;
}

p, li {
	line-height: 160%;
}

header, main, footer {
	max-width: 60em;
	margin: 2em auto;
	padding: 0 1em;
}

header {
	margin-top: 4em;
}

footer p {
	margin-top: 5em;
	font-size: 90%;
	text-align: center;
}

a:link { color: var(--link); }
a:visited { color: var(--link); }
a:hover { color: var(--link); }
a:active { color: var(--link); }

.post-info, .post-tags {
	font-size: 85%;
	color: var(--accent);
	text-align: right;
}

.post-info i:nth-child(2) {
	margin-left: .75em;
}

.tag {
	background: var(--accent);
	color: var(--background) !important;
	padding: .3em .4em;
	margin: .8em 0 0 .4em;
	border-radius: .5em;
	text-decoration: none;
	display: inline-block;
}

hr {
	border: 0;
	height: 1px;
	background: #333;
	margin: 2em 0;
}

code {
	padding: .2em .3em;
	border: 1px solid var(--accent);
	white-space: pre-wrap;
	word-wrap: break-word; 
}

pre, code {
	font-family: 'MD IO 0.4';
	font-size: 90%;
}

pre code {
	background:  #000;
	color:  #eee;
	display: inline-block;
	padding: 1em;
	white-space: pre-wrap;
	word-wrap: break-word;   
}

img {
	max-width: 100%;
}

table {
	border-collapse: collapse;
}

td, th {
	padding: .75em;
	text-align: left;
	border: 1px solid var(--accent);
}
	
.weblog-title a {
	text-decoration: none;
	color: var(--foreground);
}

form {
    display: flex;
    align-items: center;
}

input[type="text"] {
    margin-top: 0.5rem;
    border: 1px solid var(--accent);
    border-radius: 5px;
    padding: 0 10px;
    width: 265px;
    height: 30px;
    background-color: var(--background);
    color: var(--foreground);
    onchange: submit();
}

.blocked-a {
    display: block;
}

</style>
</head>
<body>

<header>
	<h1 class="weblog-title"><a href="/"><i class="fa-solid fa-house fa-sm" style="color: #fabc02;"></i> {weblog-title}</a></h1>
        <i>{weblog-description}</I>
        <br><br>
	{navigation}
</header>

<hr>

<main>

<article>
	{body}
</article>

<hr>


<h2><i class="fa-solid fa-magnifying-glass fa-sm"></i> search</h2>

<form action="?" method="get">
<label for="search"></label>
<input type="text" name="search" placeholder="type your search term and hit enter">
<input type="submit" hidden></button>
</form>

<h2><i class="fa-solid fa-wand-magic-sparkles fa-sm"></i> view other posts</h2>

<ul>
	<li><a href="/random"><i class="fa-solid fa-dice"></i> view a random post</a></li>
	<li><a href="/archive"><i class="fa-solid fa-box-archive"></i> view the posts archive</a></li>
	<li><a href="/subscribe"><i class="fa-solid fa-rss"></i> subscribe via atom/rss/json</a></li>
</ul>

</main>

<footer>
	<p>made with blood, sweat, tears, <i class="fa-solid fa-heart"></i> and <a href="https://weblog.lol">weblog.lol</a>.</p>
        <p><i>all content is copyright © {year} <a href="https://sanel.page">sanel kukic</a>. all rights reserved.</i></p>
</footer>

</body>
</html>
