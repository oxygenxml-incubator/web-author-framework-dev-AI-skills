Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface ImageHolder
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ImageHolder
An image holder that can be written to an OutputStream and contains additional information about the image.
  Since: 19.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getType](#getType())()

 void [writeTo](#writeTo(java.io.OutputStream))([OutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/OutputStream.html) out)
Writes the image to the output stream.

## Method Details

### writeTo

void writeTo([OutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/OutputStream.html) out)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Writes the image to the output stream. This method does not close the output stream. This method does not close or flush the output stream.
  Parameters: out - The output stream. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the underlying stream throws.
### getType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getType()
  Returns: The type of the image that is written, or null if the type could not be determined.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
