# How to dynamically name an object property

There are instances where you have an object in PHP that you want to add dynamically named properties to. In my case, I was populating an object that would be converting into a JSON object. Doing so requires some special syntax:

```php
$object->{"my_".$variable};
```

If you're creating dynamically named properties, you will also probably need to use `property_exists` at some point:

```
if (property_exists($object, "my_".$variable)) {
   // ...whatever
}
```


