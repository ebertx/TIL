# Formate a number using `toLocalString()`

You can easily format a number with a large degree of customizability using the method `toLocaleString()`.

For example:

```
var num = 1000;
console.log(num.toLocaleString();

// Displays '1,000'
```

The default call will display the number matching the locale as described by the OS. Parameters exists that allow you to explicitly declare a locale, or even specify if the number should be displayed as currency.

```
var num = 1000;
console.log(num.toLocaleString('en-US', { style: 'currency', currency: 'USD' });

// Displays '$1,000.00'
```

Browser support is good, but not universal.

[Source](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Number/toLocaleString)
