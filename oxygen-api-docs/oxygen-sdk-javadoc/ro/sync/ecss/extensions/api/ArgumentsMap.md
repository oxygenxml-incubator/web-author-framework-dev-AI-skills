Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface ArgumentsMap
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ArgumentsMap
Map between argument names and values.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getArgumentValue](#getArgumentValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) argumentName)
Get the value for the specified argument name.

## Method Details

### getArgumentValue

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getArgumentValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) argumentName)

Get the value for the specified argument name. The argument name must be one of the arguments defined in [AuthorOperation.getArguments()](AuthorOperation.md#getArguments()) method.
  Parameters: argumentName - The name of the argument. Returns: The value of the argument, or null if a value was not stored for the given argument.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
