Parses PHP serialized objects into Java objects.

Sample use:

```
String input = "O:8:"TypeName":1:{s:3:"foo";s:3:"bar";}";
SerializedPhpParser serializedPhpParser = new SerializedPhpParser(input);
Object result = serializedPhpParser.parse();
```

The `result` object will be a `PhpObject` with the name `TypeName` and the attribute `foo` = `bar`.

For further examples see the [test class](http://serialized-php-parser.googlecode.com/svn/trunk/test/org/lorecraft/phpserializer/SerializedPhpParserTest.java).