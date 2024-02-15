---
title: "Custom HTML5 Video Player with Vanilla JavaScript - KWG Video Player"
datePublished: Wed Jan 31 2024 07:30:13 GMT+0000 (Coordinated Universal Time)
cuid: cls2rnyfi000309k2eqjo305l
slug: custom-html5-video-player-with-vanilla-javascript-kwg-video-player

---

<div class="crayons-article__main">
            
  <iframe width="996" height="560" src="https://www.youtube.com/embed/0V1F10x9Elc" title="KWG Player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
  
  <nav class="series-switcher crayons-card crayons-card--secondary">
    <header class="crayons-card__header">
      <h2 class="crayons-subtitle-2">Custom HTML5 Video Player with Vanilla JavaScript</h2></header></nav><div class="crayons-article__body text-styles spec__body" data-article-id="980233" id="article-body">


<hr />

<p><iframe allowtransparency="true" frameborder="no" height="600" loading="lazy" scrolling="no" src="https://codepen.io/SH20RAJ/embed/oNoYZJw?height=600&amp;default-tab=result&amp;embed-version=2" style="width: 100%;">
</iframe>
</p>


<hr />

<p>KWG Video Player is a free custom HTML5 video player. It is written in Vanilla JavaScript and no library is required for it to run.<br /><br />
The video player can be used in different web projects freely. Multiple instances of the video player can be used in a single page. and the appearance of the player can be customized.  </p>

<p>Upon creating a KWG Video Player, an Object is created in which one of the members is html5 <code>&lt;video&gt;</code> element and all Media events, properties and methods are available for it.</p>

<p>For the whole functionality of <strong>KWG Video Player</strong>, see <a href="https://dev.to/plugins/custom-html5-video-player/doc">documentation source</a>.</p>
<h1>
  <a href="#integration" name="integration">
  </a>
  Integration
</h1>

<hr />

<p><strong>1. Load CDNs</strong><br />
</p>

<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;link</span> <span class="na">rel=</span><span class="s">"stylesheet"</span> <span class="na">href=</span><span class="s">"https://cdn.jsdelivr.net/gh/webgadgets/KwgVideoPlayer@master/kwg-video-player.css"</span> <span class="nt">/&gt;</span>
<span class="nt">&lt;script </span><span class="na">src=</span><span class="s">"https://cdn.jsdelivr.net/gh/webgadgets/KwgVideoPlayer@master/kwg-video-player.js"</span><span class="nt">&gt;&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p><strong>2. Set up your HTML</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video1"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
    Your browser does not support HTML5 video.
<span class="nt">&lt;/video&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<blockquote>
<p>Sample Video :- <a href="https://bit.ly/bbsamplevideo">https://bit.ly/bbsamplevideo</a></p>

<p>Sample Poster :- <a href="https://bit.ly/bbsampleposter">https://bit.ly/bbsampleposter</a></p>
</blockquote>

<p><strong>3. Initialize Player</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;script&gt;</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video1</span><span class="dl">'</span><span class="p">);</span>
<span class="nt">&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<hr />
<h2>
  <a href="#multiple-kwg-video-players-on-one-page" name="multiple-kwg-video-players-on-one-page">
  </a>
  Multiple KWG Video Players on one page
</h2>

<p><strong>Add HTML</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-1"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
<span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-2"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span><span class="nt">&gt;</span> 
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
<span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-3"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p><strong>Initialize Players</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;script&gt;</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-1</span><span class="dl">'</span><span class="p">);</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-2</span><span class="dl">'</span><span class="p">);</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-3</span><span class="dl">'</span><span class="p">);</span>
<span class="nt">&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>

<h3>
  <a href="#autoplay-video" name="autoplay-video">
  </a>
  Autoplay video
</h3>

<p><strong>Set up HTML</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-autoplay-1"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p><strong>Initialize</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;script&gt;</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-autoplay-1</span><span class="dl">'</span><span class="p">,</span> <span class="p">{</span>
        <span class="o">**</span><span class="na">autoplay</span><span class="p">:</span><span class="kc">true</span><span class="o">**</span>
    <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p>or  </p>
<h3>
  <a href="#html-video-autoplay-attribute" name="html-video-autoplay-attribute">
  </a>
  HTML video <strong>autoplay</strong> Attribute
</h3>

<p>Set up HTML</p>

<p>Copy<br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-autoplay-2"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span> <span class="na">autoplay</span><span class="err">\</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>



<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;script&gt;</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-autoplay-2</span><span class="dl">'</span><span class="p">);</span>
<span class="nt">&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>

<h3>
  <a href="#repeat-video" name="repeat-video">
  </a>
  Repeat video
</h3>

<p><strong>Set up HTML</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-repeat-1"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p><strong>Initialize</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;script&gt;</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-repeat-1</span><span class="dl">'</span><span class="p">,</span> <span class="p">{</span>
        <span class="o">**</span><span class="na">repeat</span><span class="p">:</span><span class="kc">true</span><span class="o">**</span>
    <span class="p">});</span>
<span class="nt">&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p>or  </p>

<p>HTML video <strong>loop</strong> Attribute  Like this<br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;video</span> <span class="na">id=</span><span class="s">"video-repeat-2"</span> <span class="na">width=</span><span class="s">"400"</span> <span class="na">height=</span><span class="s">"225"</span> <span class="na">loop</span><span class="err">\</span><span class="nt">&gt;</span>
    <span class="nt">&lt;source</span> <span class="na">src=</span><span class="s">"path/to/video"</span> <span class="na">type=</span><span class="s">"video/mp4"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/video&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<p><strong>Initialize</strong><br />
</p>
<div class="highlight js-code-highlight">
<pre class="highlight html"><code><span class="nt">&lt;script&gt;</span>
    <span class="k">new</span> <span class="nx">kwgVideo</span><span class="p">(</span><span class="dl">'</span><span class="s1">#video-repeat-1</span><span class="dl">'</span><span class="p">);</span>
<span class="nt">&lt;/script&gt;</span>
</code></pre>
<div class="highlight__panel js-actions-panel">
<div class="highlight__panel-action js-fullscreen-code-action">
    <svg class="highlight-action crayons-icon highlight-action--fullscreen-on" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Enter fullscreen mode</title>
    <path d="M16 3h6v6h-2V5h-4V3zM2 3h6v2H4v4H2V3zm18 16v-4h2v6h-6v-2h4zM4 19h4v2H2v-6h2v4z"></path>
</svg>

    <svg class="highlight-action crayons-icon highlight-action--fullscreen-off" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg"><title>Exit fullscreen mode</title>
    <path d="M18 7h4v2h-6V3h2v4zM8 9H2V7h4V3h2v6zm10 8v4h-2v-6h6v2h-4zM8 15v6H6v-4H2v-2h6z"></path>
</svg>

</div>
</div>
</div>


<hr />


<div class="ltag-github-readme-tag">
  <div class="readme-overview">
    <h2>
      <img alt="GitHub logo" loading="lazy" src="https://res.cloudinary.com/practicaldev/image/fetch/s--566lAguM--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev.to/assets/github-logo-5a155e1f9a670af7944dd5e12375bc76ed542ea80224905ecaf878b9157cdefc.svg" />
      <a href="https://github.com/webgadgets">
        webgadgets
      </a> / <a href="https://github.com/webgadgets/KwgVideoPlayer" style="font-weight: 600;">
        KwgVideoPlayer
      </a>
    </h2>
    <h3>
      Custom HTML5 Video Player with Vanilla JavaScript
    </h3>
  </div>
</div>



<p>Source Doc :- <a href="https://webgadgets.net/plugins/custom-html5-video-player">https://webgadgets.net/plugins/custom-html5-video-player</a></p>


          </div>

            
  <nav class="series-switcher crayons-card crayons-card--secondary">
    <header class="crayons-card__header">
      <h2 class="crayons-subtitle-2">
        <a href="/sh20raj/series/16472">JavaScript Frameworks (4 Part Series)</a>
      </h2>
    </header>

    <div class="series-switcher__list">

          <a class="crayons-link crayons-link--contentful series-switcher__link" data-preload-image="https://res.cloudinary.com/practicaldev/image/fetch/s--QuUf0wa1--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rxiaa626ku8489d9uayo.jpg" href="/sh20raj/convert-markdown-or-md-url-to-html-markdowntohtml-using-javascript-ft-showdownjs-1med" title="Published Jan 21">
            <span class="series-switcher__num">1</span>
            <span class="series-switcher__title">Convert Markdown or md URL to HTML - MarkdownToHTML - Using JavaScript ft. showdownjs</span></a></div><div class="series-switcher__list"><a class="crayons-link crayons-link--contentful series-switcher__link" data-preload-image="https://res.cloudinary.com/practicaldev/image/fetch/s--QuUf0wa1--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rxiaa626ku8489d9uayo.jpg" href="/sh20raj/convert-markdown-or-md-url-to-html-markdowntohtml-using-javascript-ft-showdownjs-1med" title="Published Jan 21">
          </a>

          <a class="crayons-link crayons-link--contentful series-switcher__link" data-preload-image="https://res.cloudinary.com/practicaldev/image/fetch/s--Xz84cWiR--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/j1tcefd9am9756jgbfhk.jpg" href="/sh20raj/fetch-github-markdown-and-show-on-blog-post-or-website-ft-showdownjs-4dm3" title="Published Jan 21">
            <span class="series-switcher__num">2</span>
            <span class="series-switcher__title">Fetch GitHub Markdown and Show on Blog Post or Website ft. showdownjs&nbsp;</span></a></div><div class="series-switcher__list"><a class="crayons-link crayons-link--contentful series-switcher__link" data-preload-image="https://res.cloudinary.com/practicaldev/image/fetch/s--Xz84cWiR--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/j1tcefd9am9756jgbfhk.jpg" href="/sh20raj/fetch-github-markdown-and-show-on-blog-post-or-website-ft-showdownjs-4dm3" title="Published Jan 21">
          </a>

          <a class="crayons-link crayons-link--contentful series-switcher__link" data-preload-image="" href="/sh20raj/webscrapperjs-get-contenthtml-of-any-website-without-being-blocked-by-cors-even-using-javascript-by-whollyapi-42l7" title="Published Jan 25">
            <span class="series-switcher__num">3</span>
            <span class="series-switcher__title">WebScrapperJS - Get Content/HTML of any website without being blocked by CORS even using JavaScript by WhollyAPI</span>&nbsp;</a></div><div class="series-switcher__list"><a class="crayons-link crayons-link--contentful series-switcher__link" data-preload-image="" href="/sh20raj/webscrapperjs-get-contenthtml-of-any-website-without-being-blocked-by-cors-even-using-javascript-by-whollyapi-42l7" title="Published Jan 25"></a><a class="crayons-link crayons-link--contentful series-switcher__link series-switcher__link--active" data-preload-image="" href="/sh20raj/custom-html5-video-player-with-vanilla-javascript-kwg-video-player-4039" title="Published Feb 6"><span class="series-switcher__num">4</span>
            <span class="series-switcher__title">Custom HTML5 Video Player with Vanilla JavaScript - KWG Video Player </span>
          </a>
    </div><div class="series-switcher__list"><br /></div><div class="series-switcher__list"><br /></div>
  </nav>

        </div>