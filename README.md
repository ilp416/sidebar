#Simple small CSS sidebar
Small, 50-css-strings, simple CSS sidebar. It can be toggled(JS) on small screens, and always showed otherwise.
##Get started

Include the library in the HEAD tag of your page:

```html 
<link rel="stylesheet" href="sidebar.css"></link>
```
        

All you need to do is have #content, #sidebar and wrap thats in .has-left-sidebar or .has-right-sidebar:
```html
<div class="has-right-sidebar">
  <div id="sidebar" ></div>
  <div id="content" ></div>
</div>
```

You can found some styles in style.css. It's not required, but usefull in most cases: setup color of sidebar, paddings, animation, some mistakes what strict eye will see.

Most likely you want to have element to toggle menu on small screens. You can add button or link and use for toggle something like this JQuery:

```html
<script>
  $(document).on('click', '.sidebar-toggler', function(){
    $(".sidebar-wrapper").toggleClass("toggled");
  });
</script>
```      

##Credits

I found and use template from http://startbootstrap.com/template-overviews/simple-sidebar/. All works were perform by them. I only simplified it, and made some cusmomizing for my tasks. Thanks. 
