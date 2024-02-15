---
title: "OpenPlayerJS - HTML5 Video/Audio/YouTube Player - Integration"
datePublished: Wed Jan 31 2024 07:28:06 GMT+0000 (Coordinated Universal Time)
cuid: cls2ro0vu000209l16yik8qml
slug: openplayerjs-html5-videoaudioyoutube-player-integration

---


<iframe width="560" height="315" src="https://www.youtube.com/embed/LS25vEByQ1g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<blockquote>
  <p>GitHub :- <a href="https://github.com/openplayerjs/openplayerjs/">https://github.com/openplayerjs/openplayerjs/</a></p>
  
  
  
<div id="driveplyr9"></div>

<script player="openplayerjs" src="https://driveplyr.appspages.online/player.js" data-id="9" data-height="555px" data-width="100%" data-type="driveplyr" defer></script>
  
  
  
  
  
  
<p>OpenPlayerJS :- <a href="https://www.openplayerjs.com/">https://www.openplayerjs.com/</a></p>
</blockquote>
<h1 id="video">Video</h1>
<pre><code class="lang-html"><span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.css"</span> /&gt;</span>
<span class="hljs-comment">&lt;!-- Adding Css CDN --&gt;</span>


  <span class="hljs-tag">&lt;<span class="hljs-name">video</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"op-player__media"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"player"</span> <span class="hljs-attr">controls</span> <span class="hljs-attr">playsinline</span> <span class="hljs-attr">width</span>=<span class="hljs-string">"100%"</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">source</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://archive.org/download/sample-video_202306/SampleVideo.mp4"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"video/mp4"</span> /&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">video</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.js"</span>&gt;</span><span class="undefined"></span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
<span class="hljs-comment">&lt;!-- Adding JavaScript CDN --&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="actionscript">
   <span class="hljs-comment">// Check the `API and events` link below for more options</span>
    <span class="hljs-keyword">const</span> player = <span class="hljs-keyword">new</span> OpenPlayerJS(<span class="hljs-string">'player'</span>);
    player.init();
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
<hr>
<h1 id="audio">Audio</h1>
<pre><code class="lang-html"><span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.css"</span> /&gt;</span>
<span class="hljs-comment">&lt;!-- Adding Css CDN --&gt;</span>


<span class="hljs-tag">&lt;<span class="hljs-name">audio</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"op-player__media"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"aud2"</span> <span class="hljs-attr">controls</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">source</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://archive.org/download/sample-video_202306/SampleVideo.mp4"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"audio/ogg"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">audio</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.js"</span>&gt;</span><span class="undefined"></span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
<span class="hljs-comment">&lt;!-- Adding JavaScript CDN --&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="actionscript">
   <span class="hljs-comment">// Check the `API and events` link below for more options</span>
    <span class="hljs-keyword">const</span> player2 = <span class="hljs-keyword">new</span> OpenPlayerJS(<span class="hljs-string">'aud2'</span>);
    player2.init();
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
<h1 id="youtube-video">YouTube Video</h1>
<pre><code class="lang-html"><span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.css"</span> /&gt;</span>
<span class="hljs-comment">&lt;!-- Adding Css CDN --&gt;</span>


        <span class="hljs-tag">&lt;<span class="hljs-name">video</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"op-player__media"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"player3"</span> <span class="hljs-attr">controls</span> <span class="hljs-attr">playsinline</span> <span class="hljs-attr">width</span>=<span class="hljs-string">"100%"</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">source</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://www.youtube.com/watch?v=xcJtL7QggTI"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"video/x-youtube"</span> /&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">video</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.js"</span>&gt;</span><span class="undefined"></span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://cdn.jsdelivr.net/npm/openplayerjs-youtube@2.3.0/dist/openplayerjs-youtube.min.js"</span>&gt;</span><span class="undefined"></span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

<span class="hljs-comment">&lt;!-- Adding JavaScript CDNs (YouTube CDN Added) --&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="actionscript">
   <span class="hljs-comment">// Check the `API and events` link below for more options</span>
    <span class="hljs-keyword">const</span> player3 = <span class="hljs-keyword">new</span> OpenPlayerJS(<span class="hljs-string">'player3'</span>);
    player3.init();
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
<h1 id="iframe">iframe</h1>
<pre><code class="lang-html">&lt;iframe src=<span class="hljs-string">"https://www.openplayerjs.com/embed.html?file=https%3A%2F%2Farchive.org%2Fdownload%2Fsample-video_202306%2FSampleVideo.mp4&amp;type=video&amp;autoplay=true"</span> style=<span class="hljs-string">"width:100%;height:700px"</span> frameborder=<span class="hljs-string">"0"</span> allow=<span class="hljs-string">"fullscreen"</span>&gt;&lt;<span class="hljs-regexp">/iframe&gt;</span>
</code></pre>
<p>Create Your iframe code Here :- <a href="https://www.openplayerjs.com/#try">https://www.openplayerjs.com/#try</a></p>
Checkout the Demo Below :-


<html>
<head>
  <title>OpenPlayerJS Examples</title>
  <link href="https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.css" rel="stylesheet"></link>
  <script src="https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.js"></script>
</head>
<body>
  <h1>OpenPlayerJS Examples</h1>

  <h2>Video</h2>
  <video class="op-player__media" controls="" id="player" playsinline="" width="100%">
    <source src="https://archive.org/download/sample-video_202306/SampleVideo.mp4" type="video/mp4"></source>
  </video>
  <hr />
  <script>
    const player = new OpenPlayerJS('player');
    player.init();
  </script>

  <h2>Audio</h2>
  <audio class="op-player__media" controls="" id="aud2">
    <source src="https://archive.org/download/sample-video_202306/SampleVideo.mp4" type="audio/ogg"></source>
  </audio>
  <hr />
  <script>
    const player2 = new OpenPlayerJS('aud2');
    player2.init();
  </script>

  <h2>YouTube Video</h2>
  <video class="op-player__media" controls="" id="player2" playsinline="" width="100%">
    <source src="https://www.youtube.com/watch?v=xcJtL7QggTI" type="video/x-youtube"></source>
  </video>
  <hr />
  <script src="https://cdn.jsdelivr.net/npm/openplayerjs-youtube@2.3.0/dist/openplayerjs-youtube.min.js"></script>
  <script>
    const player3 = new OpenPlayerJS('player2');
    player3.init();
  </script>

  <h2>iframe</h2>
  <iframe allow="fullscreen" frameborder="0" src="https://www.openplayerjs.com/embed.html?file=https%3A%2F%2Farchive.org%2Fdownload%2Fsample-video_202306%2FSampleVideo.mp4&amp;type=video&amp;autoplay=true" style="height: 700px; width: 100%;"></iframe>
</body>
</html>
