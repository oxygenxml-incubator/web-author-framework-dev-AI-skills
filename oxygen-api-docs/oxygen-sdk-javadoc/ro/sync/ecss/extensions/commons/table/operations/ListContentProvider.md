Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class ListContentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.ListContentProvider
   All Implemented Interfaces: org.eclipse.jface.viewers.IContentProvider, org.eclipse.jface.viewers.IStructuredContentProvider   @API(type=INTERNAL, src=PUBLIC) public class ListContentProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements org.eclipse.jface.viewers.IStructuredContentProvider
Empty implementation for the general purpose list (Collection) content provider.

## Constructor Summary
 Constructors
Constructor

Description
 [ListContentProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [dispose](#dispose())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [getElements](#getElements(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) inputElement)

 void [inputChanged](#inputChanged(org.eclipse.jface.viewers.Viewer,java.lang.Object,java.lang.Object))(org.eclipse.jface.viewers.Viewer viewer, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) oldInput, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) newInput)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ListContentProvider

public ListContentProvider()

## Method Details

### getElements

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] getElements([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) inputElement)
  Specified by: getElements in interface org.eclipse.jface.viewers.IStructuredContentProvider See Also:
        * IStructuredContentProvider.getElements(java.lang.Object)

### dispose

public void dispose()
  Specified by: dispose in interface org.eclipse.jface.viewers.IContentProvider See Also:
        * IContentProvider.dispose()

### inputChanged

public void inputChanged(org.eclipse.jface.viewers.Viewer viewer, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) oldInput, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) newInput)
  Specified by: inputChanged in interface org.eclipse.jface.viewers.IContentProvider See Also:
        * IContentProvider.inputChanged(org.eclipse.jface.viewers.Viewer, java.lang.Object, java.lang.Object)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
