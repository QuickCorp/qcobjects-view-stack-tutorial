# Tutorial: A View Stack Using QCObjects

## Step 1:

Create three files: view-stack.html. one.html, two.html

## Step 2:

Iside the file index.html include the following tag in the head section:

```html
<head>
<script type="text/javascript" src="https://cdn.qcobjects.dev/QCObjects.js"></script>
</head>
```

## Step 3:

In the body section, add the following:

```html
<h1>This is a view stack example</h1>
<h2>There are 3 files, view-stack.html , one.html and two.html</h2>
<h3>This part of the page (index.html) does not change when you click in a link</h3>
<p>Open DevTools in your browser (second mouse button, click on  Inspect Elements) and see what happens with the elements of this page when you click a link</p>

<component name="view-stack">
  <routing path="#one" name="page-one"></routing>
  <routing path="#two" name="page-two"></routing>
  <routing path="#" name="view-stack"></routing>
  <routing path="" name="view-stack"></routing>
</component>
```

## Step 4:

Give some style to your component

```html
<style>
component[name=view-stack]{
  border: 1px solid black;
   width: 200px;
   height: 200px;
   position: relative;
   display: block;
   padding: 0;
}
</style>
```

## The complete code looks like this

```html
<head>
<script type="text/javascript" src="https://cdn.qcobjects.dev/QCObjects.js"></script>
</head>

<body>
<style>
component[name=view-stack]{
  border: 1px solid black;
   width: 200px;
   height: 200px;
   position: relative;
   display: block;
   padding: 0;
}
</style>
<h1>This is a view stack example</h1>
<h2>There are 3 files, view-stack.html , one.html and two.html</h2>
<h3>This part of the page (index.html) does not change when you click in a link</h3>
<p>Open DevTools in your browser (second mouse button, click on  Inspect Elements) and see what happens with the elements of this page when you click a link</p>
<component name="view-stack">
<routing path="#one" name="page-one"></routing>
<routing path="#two" name="page-two"></routing>
<routing path="#" name="view-stack"></routing>
<routing path="" name="view-stack"></routing>
</component>

</body>
```

See the file [index.html](https://quickcorp.github.io/qcobjects-view-stack-tutorial/index.html) for a complete example
