<p align="right">
   <a href="https://badge.fury.io/js/@veams/component-figure"><img src="https://badge.fury.io/js/@veams/component-figure.svg" alt="npm version" height="18"></a>
    <a href="https://gitter.im/Sebastian-Fitzner/Veams?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img src="https://badges.gitter.im/Sebastian-Fitzner/Veams.svg" alt="Gitter Chat" /></a>
</p>

# Figure

## Description

The `<figure>` element is intended to be used in conjunction with the `<figcaption>` element to mark up diagrams, illustrations, photos code examples and other things. The specs says this:

> The HTML `<figure>` element represents self-contained content, frequently with a caption (`<figcaption>`), and is typically referenced as a single unit. 

The Figure component contains the picture and video component as dependency and prints out every necessary field for html figures. 

-----------

## Requirements

- [@veams/component-picture](https://github.com/Veams/component-picture) - Picture component in Veams.
- [@veams/component-video](https://github.com/Veams/component-video) - Video component in Veams.

-----------

## Installation 

### Installation with Veams

``` bash
veams install component figure
```
``` bash
veams -i c figure
```

----------- 

## Fields

### `figure.hbs`

#### Settings

| Parameter | Type | Value | Description |
|:--- |:---:|:---: |:--- |
| settings.figureContextClass | String | `default` | Context class of the figure. |
| settings.figureClasses | String | | Modifier classes for the figure. |
| settings.figureId | String | | Just pass a custom string when using an id for the figure. |

#### Content 

| Parameter | Type | Description |
|:--- |:---:|:--- |
| content.figureCaption | Object | Contains multiple elements |
| content.figureCaption.figureCaptionClasses | String | Modifier classes |
| content.figureCaption.captionHeadline | String | Headline |
| content.figureCaption.captionContent | String | Content |

##### Nested Data Fields

| Parameter | Type | Description |
|:--- |:---:|:--- 
| content.figurePicture | Object | view [@requirements](#requirements) |
| content.figureVideo | Object | view [@requirements](#requirements) |

