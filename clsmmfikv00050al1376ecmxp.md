---
title: "Adding a View Counter to Static Website with ViewCounter.io"
datePublished: Tue Feb 06 2024 04:40:21 GMT+0000 (Coordinated Universal Time)
cuid: clsmmfikv00050al1376ecmxp
slug: adding-a-view-counter-to-static-website-with-viewcounterio

---


# Adding a View Counter to Your Website with ViewCounter.io

ViewCounter.io is a service that makes it easy to add a customizable view counter to any website. With ViewCounter.io, you can:

<a id="vclink" target="_blank" href="https://visitorbadge.io/status?path=ArticlePlanet"><img id="vcimg" src="https://api.visitorbadge.io/api/visitors?path=ArticlePlanet"></a>

## Track Pageviews 

To use ViewCounter.io, you first sign up for an account and get a unique site ID. You then add the ViewCounter tracking code before the closing `</body>` tag on your pages:

```html
<script type="text/javascript">
  var viewCounter = {
    id: 12345, // your view counter ID 
    type: 'horizontal'
  }
</script>
<script type="text/javascript" src="https://api.viewcounter.io/js"></script>
```

This allows ViewCounter.io to track pageviews to your site ID on their servers.

## Display the View Count

Display your current view count anywhere on your site by adding this code:

```html 
<div data-viewcounter-id="12345"></div>
```

This will be dynamically replaced with your view count.

## Customize the Counter's Look

You can customize the counter's style, format, and messaging using parameters like:

```js
var viewCounter = {
  id: 12345,
  type: 'vertical', 
  label: 'Page Views:'
}
```

See all options: https://viewcounter.io/docs

## View Counter Analytics

In your ViewCounter.io dashboard, you can see analytics on your counter:

- Views over time
- Views by country
- Referral sources
- Recent pageviews

Dashboard: https://viewcounter.io/dashboard

## View Counter API

You can also retrieve view count data through the ViewCounter API:

```
GET https://api.viewcounter.io/count/12345
``` 

This returns the count as JSON. See API docs: https://viewcounter.io/docs/api

By handling the tracking and persistence on their servers, ViewCounter.io makes it simple to add a view counter that works across all pages of your site.