## None greedy mode

**MDN**: [Question mark](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#special-questionmark)


Example: Get all words inside <span> tag.

```js

// sample data
var input = "<span>Hello, </span><span>World</span>";

// greed mode (default mode of regular expression)
var greedyRegx = /\<span\>(.*)\<\/span\>/g;
input.match(greedyRegx);

// none-greedy mode (by using ?)
var nonegreedyRegx = /\<span\>(.*?)\<\/span\>/g;
input.match(nonegreedyRegx);
```


