Package [ro.sync.ecss.extensions.api.webapp.license](package-summary.md)

# Interface UserInfo
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface UserInfo
Information about an user.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [checkLicensed](#checkLicensed())()
Throws if the current user is not licensed.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getId](#getId())()
The user unique id.

## Method Details

### getId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getId()

The user unique id.
  Returns: The user id.
### checkLicensed

void checkLicensed()

Throws if the current user is not licensed.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
