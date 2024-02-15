---
title: "Creating a Beautiful Custom Scrollbar for Website Using CSS ✨"
datePublished: Thu Feb 01 2024 15:35:36 GMT+0000 (Coordinated Universal Time)
cuid: clsmmnc5h00040al0ffpegkqk
slug: creating-a-beautiful-custom-scrollbar-for-website-using-css

---

# Creating a Beautiful Custom Scrollbar for Your Site in Plain CSS

> See More :- https://codexdindia.blogspot.com/2024/02/creating-beautiful-custom-scrollbar-for.html


Scrollbars are an essential part of web design, providing users with a means to navigate through content. While browsers offer default scrollbars, they may not always align with your website's aesthetics. Fortunately, you can customize scrollbars with plain CSS to create a more visually appealing and cohesive design. In this tutorial, we'll guide you through the process of creating a beautiful custom scrollbar for your site.

## 1. Understanding the Basics

Before diving into customization, it's essential to understand the structure of scrollbars. Browsers interpret scrollbar styles through the `::-webkit-scrollbar` pseudo-element for WebKit-based browsers (like Chrome and Safari) and `::-moz-scrollbar` for Firefox. We'll be using both to cover a broader range of browsers.

```css
/* WebKit-based browsers */
::-webkit-scrollbar {
  width: 12px; /* Width of the scrollbar */
}

/* Firefox */
::-moz-scrollbar {
  width: 12px;
}
```

## 2. Styling the Track

The scrollbar track is the area the thumb moves along. Customize its background color, border-radius, and other properties to match your website's design.

```css
/* WebKit-based browsers */
::-webkit-scrollbar-track {
  background-color: #f1f1f1; /* Track color */
  border-radius: 10px; /* Rounded corners */
}

/* Firefox */
::-moz-scrollbar-track {
  background-color: #f1f1f1;
  border-radius: 10px;
}
```

## 3. Styling the Thumb

The thumb is the draggable part of the scrollbar. Adjust its background color, border-radius, and other properties to enhance its appearance.

```css
/* WebKit-based browsers */
::-webkit-scrollbar-thumb {
  background-color: #888; /* Thumb color */
  border-radius: 10px; /* Rounded corners */
}

/* Firefox */
::-moz-scrollbar-thumb {
  background-color: #888;
  border-radius: 10px;
}
```

## 4. Hover Effects

To make your scrollbar even more interactive, add hover effects to the thumb.

```css
/* WebKit-based browsers */
::-webkit-scrollbar-thumb:hover {
  background-color: #555; /* Hover color */
}

/* Firefox */
::-moz-scrollbar-thumb:hover {
  background-color: #555;
}
```

## 5. Changing the Cursor

Customize the cursor when hovering over the scrollbar thumb to provide visual feedback.

```css
/* WebKit-based browsers */
::-webkit-scrollbar-thumb:active {
  cursor: pointer; /* Change cursor on click */
}

/* Firefox */
::-moz-scrollbar-thumb:active {
  cursor: pointer;
}
```

## 6. Final Touches

Adjust any additional styles to fine-tune the scrollbar's appearance. For example, you can customize the corner properties and hide the scrollbar when not in use.

```css
/* WebKit-based browsers */
::-webkit-scrollbar-corner {
  background-color: #f1f1f1; /* Corner color */
}

/* Firefox */
::-moz-scrollbar-corner {
  background-color: #f1f1f1;
}

/* Hide scrollbar when not in use */
body {
  scrollbar-width: thin;
  scrollbar-color: transparent transparent;
}
```

## 7. Testing and Compatibility

After applying the styles, test your custom scrollbar across different browsers to ensure compatibility. Adjustments may be needed for specific browsers or versions.

By following these steps, you can create a beautiful custom scrollbar that complements your website's design. Experiment with colors, sizes, and other properties to achieve the desired look and feel.