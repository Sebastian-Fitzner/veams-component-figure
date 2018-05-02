## Usage

### Include: Page

``` hbs
{{! @INSERT :: START @id: figure, @tag: component-partial }}
{{#with figurp.variations.simple}}
	{{> figure}}
{{/with}}

{{#with figure.variations.caption}}
	{{> figure}}
{{/with}}

{{#with figure.variations.video}}
	{{> figure}}
{{/with}}
{{! @INSERT :: END }}
```
