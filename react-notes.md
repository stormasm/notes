

### How to convert objects to arrays for map

How to convert JSON data returned in fetch to an array that does not
have a key component already in the JSON data structure.

[noted here in stackoverflow](https://stackoverflow.com/questions/11922383/access-process-nested-objects-arrays-or-json)

```
const data = this.state.data;
const myary = [];
for (const prop in data) {
  myary.push(data[prop]);
}
```

[code from here](https://github.com/stormasm/mui-demos/blob/master/checkboxlist/src/CheckboxList-gh.js)
