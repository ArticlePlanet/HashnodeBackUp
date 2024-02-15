---
title: "Get Slug in NextJS"
datePublished: Wed Feb 14 2024 10:27:19 GMT+0000 (Coordinated Universal Time)
cuid: clsmmljiy000008k08wo15s0i
slug: get-slug-in-nextjs

---

```javascript
export default  async ({params}) => {



      let api = 'https://dev.to/api/articles/' + params.slug[0]+'/'+params.slug[1];
      let x = await fetch(api);
      let y = await x.json();

    return (
        <>
        
        <h1>Hii {y.title}</h1> 
        <p>Post: {y.body_html}</p>
        </>
    )
}
```