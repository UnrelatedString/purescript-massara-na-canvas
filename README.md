# purescript-massara-na-canvas

[![CI](https://github.com/UnrelatedString/purescript-massara-na-canvas/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/UnrelatedString/purescript-massara-na-canvas/actions/workflows/ci.yml)
![Latest Version Tag](https://img.shields.io/github/v/tag/UnrelatedString/purescript-massara-na-canvas)
[![Pursuit](https://pursuit.purescript.org/packages/purescript-massara-na-canvas/badge?)](https://pursuit.purescript.org/packages/purescript-massara-na-canvas)

> いつまでも　いくつまでも  
> 忘れないでいよう  
> まっさらなキャンバスの上  
> 描き殴るように刻むんだ

A purer, more ergonomic wrapper for the Canvas API. The aim is that all state which affects drawing operations is explicitly accounted for. Additionally, though modeled on it without excessively introducing extra power or abstractions--repackaging its existing concepts--much of the machinery is not tightly coupled to the actual Canvas API and can be mocked out or emulated without too much hassle (for example, with the Cairo-based `canvas` implementation on npm).
