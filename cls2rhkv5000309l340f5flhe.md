---
title: "Plyr.io Youtube Embedded Video Player Integration"
datePublished: Wed Jan 31 2024 07:35:10 GMT+0000 (Coordinated Universal Time)
cuid: cls2rhkv5000309l340f5flhe
slug: plyrio-youtube-embedded-video-player-integration

---

https://codexdindia.blogspot.com/2020/12/plyrio-youtube-embedded-video-player.html

---

<p><br /></p><h2 style="text-align: center;"><span style="font-size: large;">How to Play Youtube Embedded Video With Plyr.io Video Player&nbsp;</span></h2><div style="text-align: center;"><span style="font-size: medium;">See Demo on Repl :-&nbsp;<a href="https://repl.it/@SH20RAJ/PlyrVideo#index.html">https://repl.it/@SH20RAJ/PlyrVideo#index.html</a></span></div><div style="text-align: center;"><span style="font-size: large;"><br /></span></div><div><span style="font-size: large;">Video Documentation :-&nbsp;</span></div><div><span style="font-size: large;"><br /></span></div><div style="text-align: center;"><span style="font-size: large;"><iframe allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" frameborder="0" height="315" src="https://www.youtube.com/embed/jmxESAo1i28" width="560"></iframe></span></div><p><br /></p><p><br /></p><p><span style="font-size: medium;">See Latest Documentation :-&nbsp;</span></p><p></p><div class="post-header" style="-webkit-text-stroke-width: 0px; background-color: white; color: black; display: block; font-family: Ubuntu, sans-serif; font-style: normal; font-variant-caps: normal; font-variant-ligatures: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-decoration-color: initial; text-decoration-style: initial; text-decoration-thickness: initial; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; width: auto; word-spacing: 0px;"></div><p></p><div class="post-title-container" style="-webkit-text-stroke-width: 0px; background-color: white; color: black; font-family: Ubuntu, sans-serif; font-style: normal; font-variant-caps: normal; font-variant-ligatures: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-decoration-color: initial; text-decoration-style: initial; text-decoration-thickness: initial; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px;"><h3 class="post-title entry-title" style="color: #212121; font: 500 24px Ubuntu, sans-serif; margin: 0px;">Plyr.io Video Player - Integration - Skin Customizing - Adding Download Button :-&nbsp;<a href="https://codexdindia.blogspot.com/2021/05/plyrio-video-player-integration-skin-Customizing-and-Adding-Download-Button-to-plyr.html">https://codexdindia.blogspot.com/2021/05/plyrio-video-player-integration-skin-Customizing-and-Adding-Download-Button-to-plyr.html</a></h3><div style="font-size: 16px;"><br /></div><div style="font-size: 16px;"><br /></div></div><p>Step 1 :- Add CDNs&nbsp;</p><p><span>&nbsp;&nbsp; &nbsp;</span>1. Css CDN before &lt;/head&gt; Tag</p><p>

<!--Docs styles-->
<link href="https://cdn.plyr.io/3.6.3/plyr.css" rel="stylesheet"></link>
</p><pre>    <code class="language-html">
    &lt;!-- Docs styles --&gt;
    &lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/CDNSFree2/Plyr/plyr.css" /&gt;

    </code>
</pre>




<p></p><p><br /></p><p><span>&nbsp;&nbsp; &nbsp;</span>2. JS CDN before &lt;/body&gt; Tag</p><p>

</p><pre>    <code class="language-html">
&lt;script src="https://cdn.jsdelivr.net/gh/CDNSFree2/Plyr/plyr.js"&gt;&lt;/script&gt;
    </code>
</pre>








<p><br /></p><p>Step 2 :-&nbsp;</p><p><span>&nbsp; &nbsp; Insert Your YouTube iframe Code in Between these div tags :-</span><br /></p><p><span><span>&nbsp;&nbsp; &nbsp;</span><span>&nbsp; &nbsp; (Here The main thing is to add or assign id="player" to your div element)</span></span></p><p><span><span>
  
  
  
  </span></span></p>
<pre><code class="language-html">
      &lt;div style="width: 500px;" class="plyr__video-embed" id="player"&gt;
        &lt;iframe src="https://www.youtube.com/embed/bTqVqk7FSmY" 
            allowfullscreen 
            allowtransparency
            allow="autoplay"&gt;
        &lt;/iframe&gt;
    &lt;/div&gt;
    </code>
</pre><span><span>

  
  
  
  
  
  
  
  
  
  </span></span><p></p><p><span><br /></span></p><h4 style="text-align: left;"><span>Now , Your WebPage Will Look Like :-&nbsp;</span></h4><div><table align="center" cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-5br0nDXSSxA/X9xWXeA2YdI/AAAAAAAAAYI/_lNFD2o6oqMmkMnfHdZtpBnQStMAN43ZgCLcBGAsYHQ/s897/after.JPG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="506" data-original-width="897" height="362" src="https://1.bp.blogspot.com/-5br0nDXSSxA/X9xWXeA2YdI/AAAAAAAAAYI/_lNFD2o6oqMmkMnfHdZtpBnQStMAN43ZgCLcBGAsYHQ/w640-h362/after.JPG" width="640" /></a></td></tr><tr><td class="tr-caption" style="text-align: center;">After Adding Plyr</td></tr></tbody></table><br /><div class="separator" style="clear: both; text-align: center;"><br /></div><div class="separator" style="clear: both; text-align: center;"><br /></div><table align="center" cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-ybijIaka_58/X9xWYanUJRI/AAAAAAAAAYM/bx8mV1vFfHg9dA-_HACEZx0T_Cji_T5QgCLcBGAsYHQ/s1366/before_plyr.JPG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="626" data-original-width="1366" height="294" src="https://1.bp.blogspot.com/-ybijIaka_58/X9xWYanUJRI/AAAAAAAAAYM/bx8mV1vFfHg9dA-_HACEZx0T_Cji_T5QgCLcBGAsYHQ/w640-h294/before_plyr.JPG" width="640" /></a></td></tr><tr><td class="tr-caption" style="text-align: center;">Before Adding Plyr</td></tr></tbody></table><br /><span><br /></span></div><h3 style="text-align: center;">See Full Script Here :-&nbsp;</h3><p>


</p><pre>  <code class="language-html">

&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;

&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;
    &lt;title&gt;Plyr.io YouTube Embeded Video Player&lt;/title&gt;
    &lt;!-- Docs styles --&gt;
    &lt;link rel="stylesheet" href="https://cdn.plyr.io/3.6.3/demo.css" /&gt;
&lt;/head&gt;

&lt;body&gt;
    &lt;div style="width: 500px;" class="plyr__video-embed" id="player"&gt;
        &lt;iframe src="https://www.youtube.com/embed/bTqVqk7FSmY" allowfullscreen 
            allowtransparency
            allow="autoplay"&gt;
        &lt;/iframe&gt;
    &lt;/div&gt;

    &lt;script src="https://cdn.plyr.io/3.6.3/demo.js"&gt;&lt;/script&gt;


&lt;/body&gt;

&lt;/html&gt;


    </code>
</pre>




<p><br /></p><p><br /></p><p>Chats During Video Making .....</p><p>

</p><pre>  <code class="language-html">
Plyr.io Youtube Embedded Video Player 
Integration


Steps :- 
    here is official demo from plyr

Let's embed a simple video from youtube ...

Here is simple embedding ...


Let's Cutomise it with Plyr ....

Steps:-

    See my article '
    Link in Description ........

Place iframe between div tag ..
with id = player ......
Lrt's See this .......Now


Ye Our Player Is Integrated Now ,

It's Working Too Fine ....
Thanks ......
</code></pre>



<p><br /></p><p><br /></p><p><br /></p><p>




     </p><h1 style="text-align: center;">
    Plyr.io YouTube Embeded Video Player
    </h1>
    <div class="plyr__video-embed" id="player" style="width: 500px;">
    <iframe allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" frameborder="0" height="315" src="https://www.youtube.com/embed/sZz4w88hzoE" width="560"></iframe>
    </div><div class="plyr__video-embed" id="player" style="width: 500px;"><br /></div><div class="plyr__video-embed" id="player" style="width: 500px;"><br /></div><div class="plyr__video-embed" id="player" style="width: 500px;">Here Raw File Used in this Video :-&nbsp;<a href="https://github.com/LoveShade/YT-Channel-Files/blob/main/Plyr.io/plyr.html">https://github.com/LoveShade/YT-Channel-Files/blob/main/Plyr.io/plyr.html</a></div>
    


<script src="https://cdn.plyr.io/3.6.3/demo.js"></script>

<p><br /></p><p>Our Answer on StackOverFlow :-&nbsp;<a href="https://stackoverflow.com/questions/63340764/how-to-implement-plyr-js-within-a-rails-6-site/65359662#65359662">https://stackoverflow.com/questions/63340764/how-to-implement-plyr-js-within-a-rails-6-site/65359662#65359662</a></p><p><br /></p>
<div class="hidden">
    
</div><p></p><p></p><p></p><p></p><p></p><p></p>