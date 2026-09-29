Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Class DPILocation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.DPILocation
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class DPILocation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
DPI location information.

## Constructor Summary
 Constructors
Constructor

Description
 [DPILocation](#%3Cinit%3E(int,int,java.util.List))(int startLocation, int endLocation, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Long](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Long.html)> nodeIds)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getEndLocation](#getEndLocation())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Long](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Long.html)> [getNodeIds](#getNodeIds())()

 int [getStartLocation](#getStartLocation())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DPILocation

public DPILocation(int startLocation, int endLocation, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Long](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Long.html)> nodeIds)

Constructor.
  Parameters: startLocation - Start offset of the dpi. endLocation - End offset of the dpi (exclusive). nodeIds - The nodes marked by the dpi.
## Method Details

### getStartLocation

public int getStartLocation()
  Returns: Returns the start offset of the dpi.
### getEndLocation

public int getEndLocation()
  Returns: Returns the end offset of the dpi (exclusive).
### getNodeIds

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Long](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Long.html)> getNodeIds()
  Returns: Returns the nodes marked by the dpi.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
