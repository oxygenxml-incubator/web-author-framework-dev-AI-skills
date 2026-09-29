Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface Content
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Content
Interface to describe a sequence of character content that can be edited.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) [createPosition](#createPosition(int))(int offset)
Creates a position within the content.
  void [getChars](#getChars(int,int,javax.swing.text.Segment))(int where, int len, [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html) chars)
Retrieves a portion of the content into the specified [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html).
  int [getLength](#getLength())()
The length in characters of the content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getString](#getString(int,int))(int where, int len)
Fetches a string of characters contained in the content sequence.
  void [insertChars](#insertChars(int,char%5B%5D,int,int))(int where, char[] ch, int start, int length)
Inserts a sequence of characters into the content at a given offset.
  void [remove](#remove(int,int))(int where, int nitems)
Removes some portion of the content sequence.

## Method Details

### createPosition

[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) createPosition(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Creates a position within the content. The position offset is changed as the content is edited.
  Parameters: offset - The offset in the content >= 0 Returns: A new [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html). Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - For an invalid offset
### getLength

int getLength()

The length in characters of the content.
  Returns: The length >= 0
### insertChars

void insertChars(int where, char[] ch, int start, int length)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Inserts a sequence of characters into the content at a given offset.
  Parameters: where - Offset into the content to make the insertion >= 0 ch - The char buffer to insert from. start - Start of useful data in the char buffer. length - Length of useful data in the char buffer. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - thrown if the offset indicated by the where argument is not contained in the boundaries of the content character sequence.
### remove

void remove(int where, int nitems)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Removes some portion of the content sequence.
  Parameters: where - The offset into the sequence to make the removal >= 0. nitems - The number of items in the sequence to be removed >= 0. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - Thrown if the area covered by the where and nitems parameters is not contained in the content character sequence.
### getString

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getString(int where, int len)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Fetches a string of characters contained in the content sequence.
  Parameters: where - Offset into the sequence to fetch >= 0. len - Number of characters to copy >= 0. Returns: The extracted String. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - Thrown if the area covered by the arguments is not contained in the content character sequence.
### getChars

void getChars(int where, int len, [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html) chars)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Retrieves a portion of the content into the specified [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html). If the desired content spans the gap, we copy the content. If the desired content does not span the gap, the actual store is returned to avoid the copy since it is contiguous.
  Parameters: where - The starting position >= 0, where + len <= length() len - The number of characters to be retrieved >= 0 chars - The [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html) object to return the characters into. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the specified position or length are invalid.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
