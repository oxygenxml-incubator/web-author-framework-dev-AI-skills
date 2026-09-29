Package [ro.sync.exml.workspace.api.editor.page.ditamap](package-summary.md)

# Interface DITAMapNodeRendererCustomizerContext
    All Superinterfaces: [AuthorNodeRendererCustomizerContext](../author/AuthorNodeRendererCustomizerContext.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DITAMapNodeRendererCustomizerContextextends [AuthorNodeRendererCustomizerContext](../author/AuthorNodeRendererCustomizerContext.md)
Offers more information about the class of the target topics.
  Since: 19.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [TopicRefTargetInfo](../../../standalone/ditamap/TopicRefTargetInfo.md) [getTopicRefTargetInfo](#getTopicRefTargetInfo())()
Get information about the topic referenced by this topicref.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.[AuthorNodeRendererCustomizerContext](../author/AuthorNodeRendererCustomizerContext.md)
 [getAuthorNode](../author/AuthorNodeRendererCustomizerContext.md#getAuthorNode())
## Method Details

### getTopicRefTargetInfo

[TopicRefTargetInfo](../../../standalone/ditamap/TopicRefTargetInfo.md) getTopicRefTargetInfo()

Get information about the topic referenced by this topicref. May be null
  Returns: Information about this topic referenced by this topicref. May be null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
