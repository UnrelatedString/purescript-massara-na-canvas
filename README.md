# purescript-massara-na-canvas

[![CI](https://github.com/UnrelatedString/purescript-massara-na-canvas/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/UnrelatedString/purescript-massara-na-canvas/actions/workflows/ci.yml)
![Latest Version Tag](https://img.shields.io/github/v/tag/UnrelatedString/purescript-massara-na-canvas)
[![Pursuit](https://pursuit.purescript.org/packages/purescript-massara-na-canvas/badge?)](https://pursuit.purescript.org/packages/purescript-massara-na-canvas)

> いつまでも　いくつまでも  
> 忘れないでいよう  
> まっさらなキャンバスの上  
> 描き殴るように刻むんだ

A purer, more ergonomic wrapper for the Canvas API. The aim is that all state which affects drawing operations is explicitly accounted for. Additionally, though modeled on it without excessively introducing extra power or abstractions--repackaging its existing concepts--much of the machinery is not tightly coupled to the actual Canvas API and can be mocked out or emulated without too much hassle (for example, with the Cairo-based `canvas` implementation on npm).

The Canvas API bindings use types from the existing `canvas` package when possible, but otherwise are implemented with raw FFI calls. (Or maybe I shouldn't even do that...? It would still be, like, uncomfortably tight coupling.)

## Coverage:

### `HTMLCanvasElement`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLCanvasElement#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:CanvasElement)

- [ ] width
- [ ] height
- [ ] getContext
- [ ] toDataURL
- [ ] toBlob
- [ ] transferControlToOffscreen

### `CanvasRenderingContext2D`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:Context2D)

#### mixin interface `CanvasSettings`

- [ ] getContextAttributes

#### mixin interface `CanvasState`

- [ ] save
- [ ] restore
- [ ] reset
- [ ] isContextLost

#### mixin interface `CanvasTransform`

- [ ] scale
- [ ] rotate
- [ ] translate
- [ ] transform
- [ ] getTransform
- [ ] setTransform
- [ ] resetTransform

#### mixin interface `CanvasCompositing`

- [ ] globalAlpha
- [ ] globalCompositeOperation

#### mixin interface `CanvasImageSmoothing`

- [ ] imageSmoothingEnabled
- [ ] imageSmoothingQuality

#### mixin interface `CanvasFillStrokeStyles`

- [ ] strokeStyle
  - [ ] DOMString
  - [ ] CanvasGradient
  - [ ] CanvasPattern
- [ ] fillStyle
  - [ ] DOMString
  - [ ] CanvasGradient
  - [ ] CanvasPattern
- [ ] createLinearGradient
- [ ] createRadialGradient
- [ ] createConicGradient
- [ ] createPattern

#### mixin interface `CanvasShadowStyles`

- [ ] shadowOffsetX
- [ ] shadowOffsetY
- [ ] shadowBlur
- [ ] shadowColor

#### mixin interface `CanvasFilters`

- [ ] filter

#### mixin interface `CanvasRect`

- [ ] clearRect
- [ ] fillRect
- [ ] strokeRect

#### mixin interface `CanvasDrawPath`

- [ ] beginPath
- [ ] fill
- [ ] stroke
- [ ] clip
- [ ] isPointInPath
- [ ] isPointInStroke

#### mixin interface `CanvasUserInterface`

- [ ] drawFocusIfNeeded

#### mixin interface `CanvasText`

- [ ] fillText
- [ ] strokeText
- [ ] measureText

#### mixin interface `CanvasDrawImage`

- [ ] drawImage
  - [ ] dx, dy
  - [ ] sx, sy

#### mixin interface `CanvasImageData`

- [ ] createImageData
- [ ] getImageData
- [ ] putImageData

#### mixin interface `CanvasPathDrawingStyles`

- [ ] lineWidth
- [ ] lineCap
- [ ] lineJoin
- [ ] miterLimit

#### mixin interface `CanvasTextDrawingStyles`
#### mixin interface `CanvasPath`

### `CanvasGradient`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/CanvasGradient#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:CanvasGradient)


### `CanvasPattern`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/CanvasPattern#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:CanvasPattern)


### `ImageBitmap`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/ImageBitmap#specifications) (not in `purescript-canvas`)

(low priority)


### `ImageData`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/ImageData#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:ImageData)


### `TextMetrics`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/TextMetrics#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:TextMetrics)


### `OffscreenCanvas`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/OffscreenCanvas#specifications) (not in `purescript-canvas`, yet)





The above Canvas API listing is adapted from ["Canvas API"](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) by Mozilla Contributors, licensed under CC-BY-SA 2.5, and from [the HTML Living Standard](https://html.spec.whatwg.org/multipage/canvas.html) by WHATWG, licensed under CC-BY 4.0. Note to self: include similar attribution [according to such guidelines](https://developer.mozilla.org/en-US/docs/MDN/Writing_guidelines/Attrib_copyright_license) when writing my own docs!
