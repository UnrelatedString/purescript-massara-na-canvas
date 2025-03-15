# purescript-massara-na-canvas

> いつまでも　いくつまでも  
> 忘れないでいよう  
> まっさらなキャンバスの上  
> 描き殴るように刻むんだ

A purer, more ergonomic wrapper for the Canvas API. The aim is that all state which affects drawing operations is explicitly accounted for, and most drawing operations are represented as "not even monadic" but rather by a simple monoid that does not and cannot encode any kind of impure *computation* alongside the simple actions. Additionally, though modeled on it without excessively introducing extra power or abstractions--repackaging its existing concepts--much of the machinery is not tightly coupled to the actual Canvas API and can be mocked out or emulated without too much hassle (for example, with the Cairo-based `canvas` implementation on npm).

## Coverage:

### `HTMLCanvasElement`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLCanvasElement#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:CanvasElement)


### `CanvasRenderingContext2D`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:Context2D)


### `CanvasGradient`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/CanvasGradient#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:CanvasGradient)


### `CanvasPattern`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/CanvasPattern#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:CanvasPattern)


### `ImageBitmap`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/ImageBitmap#specifications) (not in `purescript-canvas`--FFI this? does it even matter)


### `ImageData`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/ImageData#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:ImageData)


### `TextMetrics`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/TextMetrics#specifications) [Pursuit](https://pursuit.purescript.org/packages/purescript-canvas/6.0.0/docs/Graphics.Canvas#t:TextMetrics)


### `OffscreenCanvas`

[MDN](https://developer.mozilla.org/en-US/docs/Web/API/OffscreenCanvas#specifications) (not in `purescript-canvas`, but this is actually like really useful so I'm actually going to PR it in)





The above Canvas API listing is adapted from ["Canvas API"](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) by Mozilla Contributors, licensed under CC-BY-SA 2.5, and from [the HTML Living Standard](https://html.spec.whatwg.org/multipage/canvas.html) by WHATWG, licensed under CC-BY 4.0. Note to self: include similar attribution [according to such guidelines](https://developer.mozilla.org/en-US/docs/MDN/Writing_guidelines/Attrib_copyright_license) when writing my own docs!
