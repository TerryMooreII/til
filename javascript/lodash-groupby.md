# LoDash groupBy

Creates an object composed of keys generated from the results of running each element of collection through iteratee. The corresponding value of each key is an array of elements responsible for generating the key. The iteratee is invoked with one argument: (value).

```javascript
_.groupBy([6.1, 4.2, 6.3], Math.floor);
// → { '4': [4.2], '6': [6.1, 6.3] }

// The `_.property` iteratee shorthand.
_.groupBy(['one', 'two', 'three'], 'length');
// → { '3': ['one', 'two'], '5': ['three'] }
```

[Source](https://lodash.com/docs#groupBy)

This is great for grouping the shows by year for an artist on the Live Music section of Archive.org API.
