Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class GetCurrentElementSaxonExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * net.sf.saxon.lib.ExtensionFunctionDefinition
        * ro.sync.ecss.extensions.commons.operations.GetCurrentElementSaxonExtension
   @API(type=INTERNAL, src=PUBLIC) public class GetCurrentElementSaxonExtension extends net.sf.saxon.lib.ExtensionFunctionDefinition
Returns the current element for an XSLT operation.

## Constructor Summary
 Constructors
Constructor

Description
 [GetCurrentElementSaxonExtension](#%3Cinit%3E(ro.sync.ecss.extensions.commons.operations.ElementLocationPath))(ro.sync.ecss.extensions.commons.operations.ElementLocationPath currentElementLocation)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 net.sf.saxon.value.SequenceType[] [getArgumentTypes](#getArgumentTypes())()

 net.sf.saxon.om.StructuredQName [getFunctionQName](#getFunctionQName())()

 net.sf.saxon.value.SequenceType [getResultType](#getResultType(net.sf.saxon.value.SequenceType%5B%5D))(net.sf.saxon.value.SequenceType[] suppliedArgumentTypes)

 net.sf.saxon.lib.ExtensionFunctionCall [makeCallExpression](#makeCallExpression())()

### Methods inherited from class net.sf.saxon.lib.ExtensionFunctionDefinition
 asFunction, dependsOnFocus, getMaximumNumberOfArguments, getMinimumNumberOfArguments, hasSideEffects, trustResultType
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### GetCurrentElementSaxonExtension

public GetCurrentElementSaxonExtension(ro.sync.ecss.extensions.commons.operations.ElementLocationPath currentElementLocation)

Constructor.
  Parameters: currentElementLocation - the location of the element defined as a simple XPath.
## Method Details

### getFunctionQName

public net.sf.saxon.om.StructuredQName getFunctionQName()
  Specified by: getFunctionQName in class net.sf.saxon.lib.ExtensionFunctionDefinition See Also:
        * ExtensionFunctionDefinition.getFunctionQName()

### getArgumentTypes

public net.sf.saxon.value.SequenceType[] getArgumentTypes()
  Specified by: getArgumentTypes in class net.sf.saxon.lib.ExtensionFunctionDefinition See Also:
        * ExtensionFunctionDefinition.getArgumentTypes()

### getResultType

public net.sf.saxon.value.SequenceType getResultType(net.sf.saxon.value.SequenceType[] suppliedArgumentTypes)
  Specified by: getResultType in class net.sf.saxon.lib.ExtensionFunctionDefinition See Also:
        * ExtensionFunctionDefinition.getResultType(net.sf.saxon.value.SequenceType[])

### makeCallExpression

public net.sf.saxon.lib.ExtensionFunctionCall makeCallExpression()
  Specified by: makeCallExpression in class net.sf.saxon.lib.ExtensionFunctionDefinition See Also:
        * ExtensionFunctionDefinition.makeCallExpression()

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
