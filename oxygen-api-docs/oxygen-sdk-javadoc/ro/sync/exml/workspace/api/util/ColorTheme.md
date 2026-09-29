Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface ColorTheme
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ColorTheme
A theme manager is an object that is able to provide information about the color theme used by oXygen. The color theme is used to style all the views and controls used by oxygen as well as the editors.
  Since: 16.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [isDarkTheme](#isDarkTheme())()
Check if the current theme is a dark theme.
  boolean [isHighContrastTheme](#isHighContrastTheme())()
Check if the current theme is a high contrast one.
  boolean [isHighContrastWhiteTheme](#isHighContrastWhiteTheme())()
Check if the current theme is a high contrast white theme.

## Method Details

### isHighContrastTheme

boolean isHighContrastTheme()

Check if the current theme is a high contrast one.
  Returns: true if is a high contrast theme. Since: 16.1
### isHighContrastWhiteTheme

boolean isHighContrastWhiteTheme()

Check if the current theme is a high contrast white theme.
  Returns: true if is a high contrast theme. Since: 16.1
### isDarkTheme

boolean isDarkTheme()

Check if the current theme is a dark theme.
  Returns: true if is a dark theme. Since: 17
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
