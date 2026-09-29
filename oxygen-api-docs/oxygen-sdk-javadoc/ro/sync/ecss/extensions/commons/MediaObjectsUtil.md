Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class MediaObjectsUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.MediaObjectsUtil
   @API(type=INTERNAL, src=PUBLIC) public final class MediaObjectsUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility methods for media objects.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [ALLOWED_MEDIA_EXTENSIONS](#ALLOWED_MEDIA_EXTENSIONS)
All the allowed extensions for an media file.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [MEDIA_AUDIO_EXTENSIONS](#MEDIA_AUDIO_EXTENSIONS)
Audio files extenstions.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [MEDIA_VIDEO_EXTENSIONS](#MEDIA_VIDEO_EXTENSIONS)
Video files Extensions.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [RECOGNIZED_MEDIA_HOSTS](#RECOGNIZED_MEDIA_HOSTS)
All accepted media hosts.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REFERENCE_ATTR_DATA](#REFERENCE_ATTR_DATA)
Attribute "data".
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REFERENCE_ATTR_DATAKEYREF](#REFERENCE_ATTR_DATAKEYREF)
Attribute "data key reference".

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static boolean [containsExtension](#containsExtension(java.lang.String,java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions)
Determine if an extension is found in an extension array.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [correctMediaEmbeddedReference](#correctMediaEmbeddedReference(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Corrects YouTube and Vimeo video references transforming the link into an embedded links.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [detectOutputclass](#detectOutputclass(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href)
Detects the output class of an media object by comparing object's href with the recognized extensions list.
  static boolean [hasAudioFormat](#hasAudioFormat(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)
Checks if the format is a supported audio format.
  static boolean [hasVideoFormat](#hasVideoFormat(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)
Checks if the format is a supported video format.
  static boolean [isAudioReference](#isAudioReference(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileName)
Checks if the extension of file name is a reference to supported audio types.
  static boolean [isEmbeddedContent](#isEmbeddedContent(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Determines if the referred resource is YouTube or Vimeo embedded content.
  static boolean [isMediaReference](#isMediaReference(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Checks if the URL is a media reference and an media object (not xref) should be inserted.
  static boolean [isRecognizedAsMedia](#isRecognizedAsMedia(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hostURL)
Determine if the host of an inserted video should be treated as media object.
  static boolean [isVideoReference](#isVideoReference(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileName)
Checks if the extension of file name is a reference to supported video types.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### REFERENCE_ATTR_DATA

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REFERENCE_ATTR_DATA

Attribute "data".
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.commons.MediaObjectsUtil.REFERENCE_ATTR_DATA)

### REFERENCE_ATTR_DATAKEYREF

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REFERENCE_ATTR_DATAKEYREF

Attribute "data key reference".
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.commons.MediaObjectsUtil.REFERENCE_ATTR_DATAKEYREF)

### MEDIA_AUDIO_EXTENSIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] MEDIA_AUDIO_EXTENSIONS

Audio files extenstions.

### MEDIA_VIDEO_EXTENSIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] MEDIA_VIDEO_EXTENSIONS

Video files Extensions.

### ALLOWED_MEDIA_EXTENSIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] ALLOWED_MEDIA_EXTENSIONS

All the allowed extensions for an media file.

### RECOGNIZED_MEDIA_HOSTS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] RECOGNIZED_MEDIA_HOSTS

All accepted media hosts.

## Method Details

### containsExtension

public static boolean containsExtension([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions)

Determine if an extension is found in an extension array.
  Parameters: extension - Searched extension. allowedExtensions - Array with the allowed extensions. Returns: true if the extension is contained.
### detectOutputclass

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) detectOutputclass([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href)

Detects the output class of an media object by comparing object's href with the recognized extensions list. If an extension is not found, the selected type is iFrame.
  Parameters: href - The file href. Returns: Detected output class.
### isMediaReference

public static boolean isMediaReference([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Checks if the URL is a media reference and an media object (not xref) should be inserted.
  Parameters: url - Resource's URL. Returns: true if the resource is a media. YouTube and Vimeo links are associated with media files.
### isEmbeddedContent

public static boolean isEmbeddedContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Determines if the referred resource is YouTube or Vimeo embedded content.
  Parameters: url - the referred resource. Returns: true if the referred resource is YouTube or Vimeo embedded video.
### isRecognizedAsMedia

public static boolean isRecognizedAsMedia([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hostURL)

Determine if the host of an inserted video should be treated as media object.
  Parameters: hostURL - Video host (like YouTube or Vimeo) Returns: true if the host is contained.
### correctMediaEmbeddedReference

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) correctMediaEmbeddedReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Corrects YouTube and Vimeo video references transforming the link into an embedded links.
```

 YouTube: From https://www.youtube.com/watch?v=video_id To https://www.youtube.com/embed/video_id
 Vimeo  : From https://vimeo.com/video_id To https://player.vimeo.com/video/video_id

```

  Parameters: url - The inserted media reference. Returns: The corrected media reference.
### isAudioReference

public static boolean isAudioReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileName)

Checks if the extension of file name is a reference to supported audio types.
  Parameters: fileName - The name of the file to check. Returns: true if current file name points to an audio file.
### hasAudioFormat

public static boolean hasAudioFormat([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)

Checks if the format is a supported audio format.
  Parameters: format - resource format. Returns: true if the format is audio.
### isVideoReference

public static boolean isVideoReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileName)

Checks if the extension of file name is a reference to supported video types.
  Parameters: fileName - The name of the file to check. Returns: true if current file name points to a video file.
### hasVideoFormat

public static boolean hasVideoFormat([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)

Checks if the format is a supported video format.
  Parameters: format - resource format. Returns: true if the format is video.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
