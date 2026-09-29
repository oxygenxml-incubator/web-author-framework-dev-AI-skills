Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorPersistentHighlight
    All Superinterfaces: [AuthorPersistentHighlightConstants](AuthorPersistentHighlightConstants.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorPersistentHighlightextends [AuthorPersistentHighlightConstants](AuthorPersistentHighlightConstants.md)
Defines the Author Persistent Highlight which get serialized in the XML as processing instruction. The Author Persistent Highlight has one of the following types defined in [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md):
*  [AuthorPersistentHighlight.PersistentHighlightType.CUSTOM_HIGHLIGHT](AuthorPersistentHighlight.PersistentHighlightType.md#CUSTOM_HIGHLIGHT) represents the Custom defined highlights that can be managed by using the [AuthorPersistentHighlighter](AuthorPersistentHighlighter.md). The name of the processing instruction markers corresponding to this type of highlight are oxy_custom_start and oxy_custom_end
*  [AuthorPersistentHighlight.PersistentHighlightType.COMMENT](AuthorPersistentHighlight.PersistentHighlightType.md#COMMENT) represents the Comment highlightswhich get serialized using the oxy_comment_start and oxy_comment_end processing instruction names.
*  [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_INSERT](AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_INSERT) represents the Insert highlight from Change Tracking, with the oxy_insert_startand oxy_insert_end corresponding processing instruction names.
*  [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_DELETE](AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_DELETE) represents the Delete highlight from Change Tracking, which get serialized by using the oxy_delete processing instruction name.
The Comment, Insert and Delete persistent highlights can be accessed and customized by using the [AuthorReviewController](../AuthorReviewController.md).
  Since: 12
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)
The Author Persistent Highlight type.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.highlights.[AuthorPersistentHighlightConstants](AuthorPersistentHighlightConstants.md)
 [ATTR_NAME_ATTRIBUTE](AuthorPersistentHighlightConstants.md#ATTR_NAME_ATTRIBUTE), [AUTHOR_NAME_ATTRIBUTE](AuthorPersistentHighlightConstants.md#AUTHOR_NAME_ATTRIBUTE), [COMMENT_ATTRIBUTE](AuthorPersistentHighlightConstants.md#COMMENT_ATTRIBUTE), [COMMENT_ID](AuthorPersistentHighlightConstants.md#COMMENT_ID), [COMMENT_PARENT_ID](AuthorPersistentHighlightConstants.md#COMMENT_PARENT_ID), [CONTENT_ATTRIBUTE](AuthorPersistentHighlightConstants.md#CONTENT_ATTRIBUTE), [DONE_ATTRIBUTE_VALUE](AuthorPersistentHighlightConstants.md#DONE_ATTRIBUTE_VALUE), [EMPTY_MARKER_ATTRIBUTE](AuthorPersistentHighlightConstants.md#EMPTY_MARKER_ATTRIBUTE), [FLAG_ATTRIBUTE](AuthorPersistentHighlightConstants.md#FLAG_ATTRIBUTE), [MID_ATTRIBUTE](AuthorPersistentHighlightConstants.md#MID_ATTRIBUTE), [MODIFICATION_TIME](AuthorPersistentHighlightConstants.md#MODIFICATION_TIME), [TYPE_ATTRIBUTE](AuthorPersistentHighlightConstants.md#TYPE_ATTRIBUTE)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorPersistentHighlight](AuthorPersistentHighlight.md) [clone](#clone(ro.sync.ecss.extensions.api.Content))([Content](../Content.md) content)
Clone the highlight to a new content.
  [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getClonedProperties](#getClonedProperties())()
Returns a copy of the internal properties map.
  int [getEndOffset](#getEndOffset())()
Get the highlight end offset.
  [Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[Map.Entry](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.Entry.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [getPropertiesIterator](#getPropertiesIterator())()
Provides an iterator over the current properties map.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getProperty](#getProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Get the value of a property
  int [getStartOffset](#getStartOffset())()
Get the highlight start offset.
  [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) [getType](#getType())()
The persistent highlight type.
  boolean [isEmpty](#isEmpty())()
Check if the marker is over content.

## Method Details

### getStartOffset

int getStartOffset()

Get the highlight start offset.
  Returns: The start offset (inclusive).
### getEndOffset

int getEndOffset()

Get the highlight end offset.
**Note:** empty persistent highlights have startOffset == endOffset & isEmpty() == true

  Returns: The end offset (inclusive).
### getClonedProperties

[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getClonedProperties()

Returns a copy of the internal properties map. The properties can contain details about the highlight author or the highlight modification timestamp, depending on the highlight type:
        * The properties names for *change tracking highlights* are: [AuthorPersistentHighlightConstants.AUTHOR_NAME_ATTRIBUTE](AuthorPersistentHighlightConstants.md#AUTHOR_NAME_ATTRIBUTE), [AuthorPersistentHighlightConstants.MODIFICATION_TIME](AuthorPersistentHighlightConstants.md#MODIFICATION_TIME)
        * For *comment highlights* the properties names are: [AuthorPersistentHighlightConstants.AUTHOR_NAME_ATTRIBUTE](AuthorPersistentHighlightConstants.md#AUTHOR_NAME_ATTRIBUTE), [AuthorPersistentHighlightConstants.MODIFICATION_TIME](AuthorPersistentHighlightConstants.md#MODIFICATION_TIME), [AuthorPersistentHighlightConstants.COMMENT_ATTRIBUTE](AuthorPersistentHighlightConstants.md#COMMENT_ATTRIBUTE) and [AuthorPersistentHighlightConstants.COMMENT_PARENT_ID](AuthorPersistentHighlightConstants.md#COMMENT_PARENT_ID) (if it is a reply)
        * Both *comment highlights* and *insert and delete highlights* can also have the [AuthorPersistentHighlightConstants.COMMENT_ID](AuthorPersistentHighlightConstants.md#COMMENT_ID) property set
        * The properties for *custom persistent highlights* are specified when the highlight is added (@see [AuthorPersistentHighlighter.addHighlight(int, int, LinkedHashMap)](AuthorPersistentHighlighter.md#addHighlight(int,int,java.util.LinkedHashMap))) and can be changed using the [AuthorPersistentHighlighter.setProperties(AuthorPersistentHighlight, LinkedHashMap)](AuthorPersistentHighlighter.md#setProperties(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.LinkedHashMap))method.

  Returns: The copy of highlight properties.
### getType

[AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) getType()

The persistent highlight type.
  Returns: The [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) corresponding to this author persistent highlight.
### isEmpty

boolean isEmpty()

Check if the marker is over content.
  Returns: true if the marker is not over any content.
### clone

[AuthorPersistentHighlight](AuthorPersistentHighlight.md) clone([Content](../Content.md) content)throws [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html)

Clone the highlight to a new content.
  Parameters: content - The new content in which to clone the current highlight. Returns: The clone of the hightlight. Never null Throws: [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html) - If various errors are encountered during the cloning procedure Since: 21.1
### getPropertiesIterator

[Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[Map.Entry](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.Entry.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> getPropertiesIterator()

Provides an iterator over the current properties map.
  Returns: iterator over the current properties map. Since: 24
### getProperty

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Get the value of a property
  Parameters: key - The property key. Returns: The property value or null. Since: 24
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
