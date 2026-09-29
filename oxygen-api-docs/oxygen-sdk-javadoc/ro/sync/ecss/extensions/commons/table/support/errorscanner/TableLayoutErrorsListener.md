Package [ro.sync.ecss.extensions.commons.table.support.errorscanner](package-summary.md)

# Class TableLayoutErrorsListener<E>

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener<E>
   Type Parameters: E - Table elements.   @API(type=INTERNAL, src=PUBLIC) public abstract class TableLayoutErrorsListener<E> extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Listener to table layout problems
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [TableLayoutErrorsListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [add](#add(E,E,ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutProblem))([E](TableLayoutErrorsListener.md) element, [E](TableLayoutErrorsListener.md) table, [TableLayoutProblem](TableLayoutProblem.md) problem)
A table layout problem encountered.
  abstract void [add](#add(E,E,ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutProblem,java.lang.Object...))([E](TableLayoutErrorsListener.md) element, [E](TableLayoutErrorsListener.md) table, [TableLayoutProblem](TableLayoutProblem.md) problem, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)... additionalMessageInfo)
A table layout problem encountered.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableLayoutErrorsListener

public TableLayoutErrorsListener()

## Method Details

### add

public abstract void add([E](TableLayoutErrorsListener.md) element, [E](TableLayoutErrorsListener.md) table, [TableLayoutProblem](TableLayoutProblem.md) problem, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)... additionalMessageInfo)

A table layout problem encountered.
  Parameters: element - The element that generated the layout problem. table - The scanned table problem - Specific table layout problem. additionalMessageInfo - Additional message information.
### add

public void add([E](TableLayoutErrorsListener.md) element, [E](TableLayoutErrorsListener.md) table, [TableLayoutProblem](TableLayoutProblem.md) problem)

A table layout problem encountered.
  Parameters: element - The element that generated the layout problem. table - The scanned table. problem - Specific table layout problem.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
