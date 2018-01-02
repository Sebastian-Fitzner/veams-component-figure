## Usage

### Include: Page

``` hbs
{{! @INSERT :: START @id: figure, @tag: component-partial }}
{{#with figure-bp.simple}}
	{{> figure}}
{{/with}}

{{#with figure-bp.caption}}
	{{> figure}}
{{/with}}

{{#with figure-bp.video}}
	{{> figure}}
{{/with}}
{{! @INSERT :: END }}
```