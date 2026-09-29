Package [ro.sync.exml.workspace.api.standalone.ditamap](package-summary.md)

# Interface TopicRefTargetInfoProvider
    @API(type=EXTENDABLE, src=PUBLIC) public interface TopicRefTargetInfoProvider
Provides information about targets for each topic reference.
  Since: 12.2
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 default void [clearCache](#clearCache())()
Invalidate the entire cache.
  void [computeTopicRefTargetInfo](#computeTopicRefTargetInfo(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[TopicRefInfo](TopicRefInfo.md),[TopicRefTargetInfo](TopicRefTargetInfo.md)> ditaMapTargetReferences)
Call back received to compute for each [TopicRefInfo](TopicRefInfo.md) key the correct properties of the [TopicRefTargetInfo](TopicRefTargetInfo.md) object.

## Method Details

### computeTopicRefTargetInfo

void computeTopicRefTargetInfo([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[TopicRefInfo](TopicRefInfo.md),[TopicRefTargetInfo](TopicRefTargetInfo.md)> ditaMapTargetReferences)

Call back received to compute for each [TopicRefInfo](TopicRefInfo.md) key the correct properties of the [TopicRefTargetInfo](TopicRefTargetInfo.md) object. The [TopicRefTargetInfo](TopicRefTargetInfo.md) values are initialized but contain no properties inside. After the call back, the map is used by Oxygen to show titles for each topic reference in the DITA Maps Manager view.
  Parameters: ditaMapTargetReferences - A map of topic references.
### clearCache

default void clearCache()

Invalidate the entire cache. Called when the entire cache needs to be invalidated, for example when F5 is pressed in the DITA maps manager view.
  Since: 22
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
