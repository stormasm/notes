

### How to convert objects to arrays for map

How to convert JSON data returned in fetch to an array that does not
have a key component already in the JSON data structure.

[Here is the problem stated in stackoverflow](https://stackoverflow.com/questions/30142361/react-js-uncaught-typeerror-this-props-data-map-is-not-a-function)

summarized here...

The .map function is only available on arrays.

It looks like data isn't in the format you are expecting it to be

**it is {} but you are expecting []**

The javascript explanation of how the code should be...

[noted here in stackoverflow](https://stackoverflow.com/questions/11922383/access-process-nested-objects-arrays-or-json)

```
const data = this.state.data;
const myary = [];
for (const prop in data) {
  myary.push(data[prop]);
}
```

[code from here](https://github.com/stormasm/mui-demos/blob/master/checkboxlist/src/CheckboxList-gh.js)

#### Another solution

Output an array of objects
like in the example repo
[graphql-redis-github](https://github.com/stormasm/graphql-redis-github)

Or see an example of the outputted data in
[ghdata](https://github.com/stormasm/ghdata)

Then in the react state variable declare the data to be array
as defined in **DataViewWrapper** inside
[ghw-menu](https://github.com/stormasm/ghw-menu)

```
this.state = {
  data: [],
  isLoading: false,
  error: null,
  repoName: repoMap[repo],
  viewName: view
};
```
