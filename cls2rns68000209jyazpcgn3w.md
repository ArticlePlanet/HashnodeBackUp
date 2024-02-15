---
title: "Plyr.io Video Player - Integration - Skin Customizing - Adding Download Button"
datePublished: Wed Jan 31 2024 07:32:40 GMT+0000 (Coordinated Universal Time)
cuid: cls2rns68000209jyazpcgn3w
slug: plyrio-video-player-integration-skin-customizing-adding-download-button

---

https://codexdindia.blogspot.com/2021/05/plyrio-video-player-integration-skin-Customizing-and-Adding-Download-Button-to-plyr.html

<p style="text-align: center;">
  <span style="font-size: x-large;">Plyr.io Video Player - Integration - Skin Customizing - Adding Download
    Button</span>
</p>
<div style="text-align: center;"><iframe allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" frameborder="0" height="409" src="https://www.youtube.com/embed/-MXgsooMKfA" title="YouTube video player" width="727"></iframe></div><br />
<iframe allowfullscreen="true" allowtransparency="true" frameborder="no" height="317" loading="lazy" scrolling="no" src="https://codepen.io/SH20RAJ/embed/abJdPPP?height=317&amp;theme-id=dark&amp;default-tab=html,result" style="width: 100%;" title="Plyr.io Video Player - Skin Customizing to pink">
  See the Pen
  <a href="https://codepen.io/SH20RAJ/pen/abJdPPP"
    >Plyr.io Video Player - Skin Customizing to pink</a
  >
  by SH20RAJ (<a href="https://codepen.io/SH20RAJ">@SH20RAJ</a>) on
  <a href="https://codepen.io">CodePen</a>.
</iframe>

<span><br />
  <br /><span style="font-size: large;">Integration :-&nbsp;</span></span><div><span><span style="font-size: large;"><br /></span></span></div><div><span><span style="font-size: large;">or Get Plyr CDNS From <a href="https://cdnjs.com/libraries/plyr" rel="nofollow" target="_blank">CDNJS Plyr</a><br /> </span>
  <pre>    <code class="language-html">
&lt;!-- Docs styles --&gt;
&lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/CDNSFree2/Plyr/plyr.css" /&gt;</code></pre>
    
    or Use CDNJS for CDN
    <pre><code class="language-html">&lt;link rel="stylesheet" href="</code>https://cdnjs.cloudflare.com/ajax/libs/plyr/3.6.7/plyr.min.css" /&gt;</pre>
    <pre><code class="language-html">
&lt;!--Add a Simple HTML5 Video tag--&gt;
  &lt;video controls data-poster="https://cdn.plyr.io/static/demo/View_From_A_Blue_Moon_Trailer-HD.jpg" class="vid1"&gt;
    &lt;!-- Video files --&gt;
    &lt;source src="https://rebrand.ly/sample-video" type="video/mp4" size="576" /&gt;
  &lt;/video&gt;

&lt;script src="https://cdnjs.cloudflare.com/ajax/libs/plyr/3.6.7/plyr.min.js"&gt;&lt;/script&gt;

&lt;script&gt;
  const player = new Plyr('.vid1');
&lt;/script&gt;

</code>
    </pre>

  <span style="font-size: large;">Skin Customising</span></span>
<div>
  <span><br /><br /><span style="font-size: medium;">Links :-&nbsp;</span></span>
</div>
<div>
  <span><span style="font-size: medium;">&nbsp; &nbsp; Plyr.io Website :-
      <a href="https://plyr.io">https://plyr.io</a>/</span></span>
</div>
<div>
  <span><span style="font-size: medium;">&nbsp; &nbsp;
      <a href="https://github.com/sampotts/plyr" rel="nofollow" target="_blank">GitHub</a>
      &amp; Documentation :-&nbsp;<a href="https://github.com/sampotts/plyr#html">https://github.com/sampotts/plyr#html</a><br /></span><br /><span style="font-size: medium;">Go To GitHub Link and See the readme.md for the documentation.</span></span>
</div>
<div>
  <span><span style="font-size: medium;"><br /></span></span>
</div>
<div>
  <span><span style="font-size: medium;"><br /></span></span>
</div>
<div style="text-align: center;">
  <span style="font-size: medium;">See All Classes Here :-&nbsp;<a href="https://github.com/sampotts/plyr#customizing-the-css" rel="nofollow" target="_blank">Customizing&nbsp;With Css</a></span>
</div>
<div style="text-align: center;"><br /></div>
<div><br /></div>
<div><span style="font-size: large;">Adding Download Button</span></div>
<div>
   <pre>    <code class="language-javascript">
  var controls =
[
    'play-large', // The large play button in the center
    'restart', // Restart playback
    'rewind', // Rewind by the seek time (default 10 seconds)
    'play', // Play/pause playback
    'fast-forward', // Fast forward by the seek time (default 10 seconds)
    'progress', // The progress bar and scrubber for playback and buffering
    'current-time', // The current time of playback
    'duration', // The full duration of the media
    'mute', // Toggle mute
    'volume', // Volume control
    'captions', // Toggle captions
    'settings', // Settings menu
    'pip', // Picture-in-picture (currently Safari only)
    'airplay', // Airplay (currently Safari only)
    'download', // Show a download button with a link to either the current source or a custom URL you specify in your options
    'fullscreen' // Toggle fullscreen
];

var player = new Plyr('#player', { controls });
  
</code>
    </pre>
</div>
<div><span style="font-size: medium;">Add this code to get All Player Controls. Add or Remove Controls From the Array to See the controls.</span></div>
<div>
  <span><span style="font-size: medium;">See Demo :-&nbsp;<a href="https://codepen.io/SH20RAJ/pen/abJdPPP">https://codepen.io/SH20RAJ/pen/abJdPPP</a></span></span>
</div>
<!--Docs styles-->
<link href="https://cdnjs.cloudflare.com/ajax/libs/plyr/3.6.7/plyr.min.css" rel="stylesheet"></link>

<!--Add a Simple HTML5 Video tag-->
<div id="container">
  <video class="vid1" controls="" data-poster="https://cdn.plyr.io/static/demo/View_From_A_Blue_Moon_Trailer-HD.jpg">
    <!-- Video files -->
    <source size="576" src="https://bit.ly/bbsamplevideo" type="video/mp4"></source>

    <!-- Caption files -->
    <track default="" kind="captions" label="English" src="https://cdn.plyr.io/static/demo/View_From_A_Blue_Moon_Trailer-HD.en.vtt" srclang="en"></track>
    <track kind="captions" label="Français" src="https://cdn.plyr.io/static/demo/View_From_A_Blue_Moon_Trailer-HD.fr.vtt" srclang="fr"></track>

  </video>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/plyr/3.6.7/plyr.min.js"></script>

<script>
  var controls =
[
    'play-large', // The large play button in the center
   // 'restart', // Restart playback
   // 'rewind', // Rewind by the seek time (default 10 seconds)
    'play', // Play/pause playback
    'fast-forward', // Fast forward by the seek time (default 10 seconds)
    'progress', // The progress bar and scrubber for playback and buffering
    'current-time', // The current time of playback
    'duration', // The full duration of the media
    'mute', // Toggle mute
    'volume', // Volume control
    'captions', // Toggle captions
    'settings', // Settings menu
    'pip', // Picture-in-picture (currently Safari only)
    'airplay', // Airplay (currently Safari only)
    'download', // Show a download button with a link to either the current source or a custom URL you specify in your options
    'fullscreen' // Toggle fullscreen
];

  const player = new Plyr('.vid1',{controls});
</script>

<style>
  :root {
  --plyr-color-main: #e657ff;
    --plyr-video-control-color	:#e8ffba;
}

</style>

<div>
  <span><span style="font-size: medium;"><br /></span></span>
</div>
<div><br /></div>
</div>