Package [ro.sync.exml.workspace.api.templates](package-summary.md)

# Interface TemplateManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TemplateManager
Utilities related to providing new file templates...
  Since: 18
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [SHOW_ARCHIVE_TEMPLATES](#SHOW_ARCHIVE_TEMPLATES)
Show archive templates only
  static final int [SHOW_DEFAULTS](#SHOW_DEFAULTS)
Show defaults only
  static final int [SHOW_ECLIPSE_DEFAULTS](#SHOW_ECLIPSE_DEFAULTS)
Show Eclipse defaults only
  static final int [SHOW_FILE_TEMPLATES](#SHOW_FILE_TEMPLATES)
Show file templates only
  static final int [SHOW_ONLY_DITA_TEMPLATES](#SHOW_ONLY_DITA_TEMPLATES)
Show only DITA templates (the ones with "dita" type set in properties or with no type specified)
  static final int [SHOW_RECENTLY_USED](#SHOW_RECENTLY_USED)
Show recently used templates only

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TemplatesCategory](TemplatesCategory.md)> [getAllTemplatesCategories](#getAllTemplatesCategories(int))(int templateToShow)
Get the templates categories.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TemplatesCategory](TemplatesCategory.md)> [getTemplatesFromConfigs](#getTemplatesFromConfigs(java.util.List,int))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.workspace.api.options.ConfigResource> configs, int templateToShow)
Get the templates categories from a list of config resources.

## Field Details

### SHOW_DEFAULTS

static final int SHOW_DEFAULTS

Show defaults only
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.templates.TemplateManager.SHOW_DEFAULTS)

### SHOW_FILE_TEMPLATES

static final int SHOW_FILE_TEMPLATES

Show file templates only
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.templates.TemplateManager.SHOW_FILE_TEMPLATES)

### SHOW_ARCHIVE_TEMPLATES

static final int SHOW_ARCHIVE_TEMPLATES

Show archive templates only
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.templates.TemplateManager.SHOW_ARCHIVE_TEMPLATES)

### SHOW_RECENTLY_USED

static final int SHOW_RECENTLY_USED

Show recently used templates only
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.templates.TemplateManager.SHOW_RECENTLY_USED)

### SHOW_ECLIPSE_DEFAULTS

static final int SHOW_ECLIPSE_DEFAULTS

Show Eclipse defaults only
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.templates.TemplateManager.SHOW_ECLIPSE_DEFAULTS)

### SHOW_ONLY_DITA_TEMPLATES

static final int SHOW_ONLY_DITA_TEMPLATES

Show only DITA templates (the ones with "dita" type set in properties or with no type specified)
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.templates.TemplateManager.SHOW_ONLY_DITA_TEMPLATES)

## Method Details

### getAllTemplatesCategories

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TemplatesCategory](TemplatesCategory.md)> getAllTemplatesCategories(int templateToShow)

Get the templates categories.
  Parameters: templateToShow - Bit level OR between:
        * [SHOW_DEFAULTS](#SHOW_DEFAULTS)
        * [SHOW_FILE_TEMPLATES](#SHOW_FILE_TEMPLATES)
        * [SHOW_ARCHIVE_TEMPLATES](#SHOW_ARCHIVE_TEMPLATES)
        * [SHOW_RECENTLY_USED](#SHOW_RECENTLY_USED)
        * [SHOW_ECLIPSE_DEFAULTS](#SHOW_ECLIPSE_DEFAULTS)
        * [SHOW_ONLY_DITA_TEMPLATES](#SHOW_ONLY_DITA_TEMPLATES)
 Returns: The available templates categories.
### getTemplatesFromConfigs

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TemplatesCategory](TemplatesCategory.md)> getTemplatesFromConfigs([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.workspace.api.options.ConfigResource> configs, int templateToShow)

Get the templates categories from a list of config resources.
  Parameters: configs - The config resources to convert to templates. templateToShow - Bit level OR between:
        * [SHOW_DEFAULTS](#SHOW_DEFAULTS)
        * [SHOW_FILE_TEMPLATES](#SHOW_FILE_TEMPLATES)
        * [SHOW_ARCHIVE_TEMPLATES](#SHOW_ARCHIVE_TEMPLATES)
        * [SHOW_RECENTLY_USED](#SHOW_RECENTLY_USED)
        * [SHOW_ECLIPSE_DEFAULTS](#SHOW_ECLIPSE_DEFAULTS)
        * [SHOW_ONLY_DITA_TEMPLATES](#SHOW_ONLY_DITA_TEMPLATES)
 Returns: The available templates categories from the specified config resources. Since: 28.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
