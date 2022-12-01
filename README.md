# tablejs

Download tjs-i.min.js (note: sanatize any user input)<br><br>
Basic example:

```js

let data = {
  headers: ["Name", "Age", "Job"],
  data: [
    {
      Name: "Michael", //can contain an html tag
      Age: 26,
      Job: "Meteorologist" 
      //all in right order
    },
    {
      Name: "Jack",
      Job: "Electrician",
      Age: 30
      //but it doesn't have to be!
    },
  ]
}

let styling = {
  borders: true,
  table: "width: 400px; height: 50px;",
  tr: "border: 1px solid black; padding: 5px;",
  td: "border: 1px solid black; padding: 5px;",
  th: "border: 1px solid black; padding: 5px;"
}

let t = new Table(data,styling);
t.append(document.body);
```
