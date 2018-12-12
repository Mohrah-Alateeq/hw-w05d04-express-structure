# Palettes Show Page

Show pages give us specific details about a given item of data. We can access different attributes from the data we sent to view by using the name of the key surrounded by curly braces. 

## How to render data:
```html
 {{#cp}}
    <h1>{{cp.subject}}</h1>
    <h1>{{cp.content}}</h1>
    {{/cp}}
```

Generally there is also a way to delete the showed data. This requires a form:

### Method: 
### Action:
 <form action="/palette/{{id}}?_method=DELETE" method="POST">
      <button type="submit">delete list</button>
    </form>
We also want to show all of the colors here. How can we do that?
<a href="/color">show all color </a>
```html 
```


<body>  <a href="/palette">back</a>
    {{#cp}}
    <h1>{{cp.subject}}</h1>
    <h1>{{cp.content}}</h1>
    {{/cp}}
    <form action="/palette/{{id}}?_method=DELETE" method="POST">
      <button type="submit">delete list</button>
    </form>
  