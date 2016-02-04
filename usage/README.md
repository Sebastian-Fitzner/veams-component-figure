# Figure

This blueprint is based on the blueprint of Veams-Components.

## Usage

### Include: Page

``` hbs
{{! @INSERT :: START @id: figure, @tag: component }}
{{#with figure-bp.simple}}
	{{> c-figure}}
{{/with}}

{{#with figure-bp.caption}}
	{{> c-figure}}
{{/with}}

{{#with figure-bp.video}}
	{{> c-figure}}
{{/with}}
{{! @INSERT :: END }}
```

### Include: SCSS

``` scss
// @INSERT :: START @id: scss-import, @tag: component
@import "components/_c-figure";
// @INSERT :: END
```
