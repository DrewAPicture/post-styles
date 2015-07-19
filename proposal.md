# Post Format Views

## Concept

One of the primary failings of how post formats were implemented when introduced, was the lack of a baseline of how content assigned to one fo those formats might be treated. We would propose to introduce base templates for ahow to display each of the default post formats; this would take the form of a core-supplied template part callable (and overrideable) by the theme.

Result: Give themes a baseline template for how post formats could be treated in a theme to highlight sections of content tagged as a particular post format.

## Affected APIs
* Post Formats
* Template Hierarchy
* Themes (template parts)

## Premise

Provide a core-supplied default template parts used tied to individual post formats. Like files provided in wpinc/theme-compat/, these template parts could be loaded by the theme by name, or optionally overridden by a theme.

## Goals
* Create core-supported base template parts for each established post format
* Deprecate less-common post formats
* Open up extending post formats in an automagical way