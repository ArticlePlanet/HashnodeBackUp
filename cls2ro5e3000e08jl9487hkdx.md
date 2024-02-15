---
title: "Disable Download option in HTML5 Video"
datePublished: Wed Jan 31 2024 07:08:19 GMT+0000 (Coordinated Universal Time)
cuid: cls2ro5e3000e08jl9487hkdx
slug: disable-download-option-in-html5-video

---

  See Video Documentation :- 

   

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706764757105/3985614d-cc2a-4d2b-a1a7-d2e1abcfed74.jpeg)](https://1.bp.blogspot.com/-enIkswl5Cew/YA5OGmLnNkI/AAAAAAAAAeQ/fobyWsrKE0YgFzgi-DFmkXJTtvYF23BhACLcBGAsYHQ/s323/Capture.JPG)

Before - When video tag Download is Enabled .

  

  

Here is a Simple Video Tag :- 
```

    <video width\="320" height\="240" controls loop\>

        <source src\="https://www.w3schools.com/tags/movie.mp4" type\="video/mp4"\>

        Your browser does not support the video tag.

    </video\>
```

\-- Preview --

 Your browser does not support the video tag.  

  

For Disabling the Download Option 

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706764758642/17b717b8-9e5c-4c5e-b032-07e9a60d8fa5.jpeg)](https://1.bp.blogspot.com/-S2DBz4kji04/YA5QqgcbOoI/AAAAAAAAAec/mxFAKansBIUC1IKjjuh0TlWcU_aPtgR5ACLcBGAsYHQ/s323/Capture.JPG)

After Disabling Download

  

Add This Attribute 

`controlslist\="nodownload"`

Now the Full Code Will Look Like :- 
```
    <video width\="320" height\="240" controls loop controlslist\="nodownload"\>

        <source src\="https://www.w3schools.com/tags/movie.mp4" type\="video/mp4"\>

        Your browser does not support the video tag.

    </video\>
```
\-- Preview --

 Your browser does not support the video tag.  
  

  

Possible controlslist Values :- 

*   nofullscreen
*   nodownload
*   noremoteplayback

  

Download Files Used in This Video :-  [https://github.com/CXDI/youtube-files/blob/main/Tips/Disable\_Download\_option\_in\_HTML5\_Video.html](https://github.com/CXDI/youtube-files/blob/main/Tips/Disable_Download_option_in_HTML5_Video.html)