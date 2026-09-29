Package [ro.sync.util.editorvars](package-summary.md)

# Enum Class EditorVariables.FrameworkRewritePolicy

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md)>
        * ro.sync.util.editorvars.EditorVariables.FrameworkRewritePolicy
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   Enclosing class: [EditorVariables](EditorVariables.md)   public static enum EditorVariables.FrameworkRewritePolicy extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md)>
Used to determine how framework variables should be expanded/rewritten.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [REWRITE_ABSOLUTE](#REWRITE_ABSOLUTE)
All framework variables will be expanded to their absolute paths.
  [REWRITE_BASE_WITH_FRAMEWORK](#REWRITE_BASE_WITH_FRAMEWORK)
Variables BASE_FRAMEWORK_DIRECTORY and BASE_FRAMEWORK_DIRECTORY_URL will be expanded to FRAMEWORK_DIRECTORY and FRAMEWORK_URL if they match.
  [REWRITE_BASE_WITH_FRAMEWORK_NAME](#REWRITE_BASE_WITH_FRAMEWORK_NAME)
Variables BASE_FRAMEWORK_DIRECTORY and BASE_FRAMEWORK_DIRECTORY_URL will be expanded to FRAMEWORK_DIR_FUNCTION_VARIABLE_PREFIX and FRAMEWORK_FUNCTION_VARIABLE_PREFIX if they match.
  [REWRITE_FRAMEWORK_WITH_BASE](#REWRITE_FRAMEWORK_WITH_BASE)
Variables FRAMEWORK_DIRECTORY and FRAMEWORK_URL will be expanded to BASE_FRAMEWORK_DIRECTORY and BASE_FRAMEWORK_DIRECTORY_URL if they match.
  [REWRITE_WITH_FRAMEWORK](#REWRITE_WITH_FRAMEWORK)
Variables FRAMEWORK_DIRECTORY and FRAMEWORK_URL will not be expanded and will be used to rewrite FRAMEWORKS_DIRECTORY and FRAMEWORKS_DIRECTORY_URL if they match.
  [REWRITE_WITH_FRAMEWORKS](#REWRITE_WITH_FRAMEWORKS)
Variables FRAMEWORKS_DIRECTORY and FRAMEWORKS_DIRECTORY_URL will not be expanded and will be used to rewrite FRAMEWORK_DIRECTORY and FRAMEWORK_URL if encountered and if they match.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### REWRITE_ABSOLUTE

public static final [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) REWRITE_ABSOLUTE

All framework variables will be expanded to their absolute paths.

### REWRITE_WITH_FRAMEWORKS

public static final [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) REWRITE_WITH_FRAMEWORKS

Variables FRAMEWORKS_DIRECTORY and FRAMEWORKS_DIRECTORY_URL will not be expanded and will be used to rewrite FRAMEWORK_DIRECTORY and FRAMEWORK_URL if encountered and if they match. If they don't match, FRAMEWORK_DIRECTORY and FRAMEWORK_URL will be expanded to their absolute paths.

### REWRITE_WITH_FRAMEWORK

public static final [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) REWRITE_WITH_FRAMEWORK

Variables FRAMEWORK_DIRECTORY and FRAMEWORK_URL will not be expanded and will be used to rewrite FRAMEWORKS_DIRECTORY and FRAMEWORKS_DIRECTORY_URL if they match. If they don't match, FRAMEWORKS_DIRECTORY and FRAMEWORKS_DIRECTORY_URL will be expanded to their absolute path.

### REWRITE_FRAMEWORK_WITH_BASE

public static final [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) REWRITE_FRAMEWORK_WITH_BASE

Variables FRAMEWORK_DIRECTORY and FRAMEWORK_URL will be expanded to BASE_FRAMEWORK_DIRECTORY and BASE_FRAMEWORK_DIRECTORY_URL if they match.

### REWRITE_BASE_WITH_FRAMEWORK

public static final [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) REWRITE_BASE_WITH_FRAMEWORK

Variables BASE_FRAMEWORK_DIRECTORY and BASE_FRAMEWORK_DIRECTORY_URL will be expanded to FRAMEWORK_DIRECTORY and FRAMEWORK_URL if they match.

### REWRITE_BASE_WITH_FRAMEWORK_NAME

public static final [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) REWRITE_BASE_WITH_FRAMEWORK_NAME

Variables BASE_FRAMEWORK_DIRECTORY and BASE_FRAMEWORK_DIRECTORY_URL will be expanded to FRAMEWORK_DIR_FUNCTION_VARIABLE_PREFIX and FRAMEWORK_FUNCTION_VARIABLE_PREFIX if they match.

## Method Details

### values

public static [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
