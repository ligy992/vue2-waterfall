# vue2-waterfall

[![Build Status](https://travis-ci.org/PLDaily/vue2-waterfall.svg?branch=master)](https://travis-ci.org/PLDaily/vue2-waterfall)
[![npm](https://img.shields.io/npm/v/vue2-waterfall.svg)](https://www.npmjs.com/package/vue2-waterfall)
[![npm](https://img.shields.io/npm/dt/vue2-waterfall.svg)](https://www.npmjs.com/package/vue2-waterfall)
[![npm](https://img.shields.io/npm/l/vue2-waterfall.svg)](https://www.npmjs.com/package/vue2-waterfall)
[![npm](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://github.com/standard/standard)

## Overview
> A waterfall or Masonry Component For Vue2

[demo](http://67.218.146.247:8088/)

## Install

### Install vue2-waterfall

```sh
npm install vue2-waterfall
```

### Import vue2-waterfall

ES6/commonjs import style is supported.

```js
// ES6
import {Waterfall, WaterfallItem} from 'vue2-waterfall';

// commonjs
const Waterfall = require("vue2-waterfall").Waterfall;
const WaterfallItem = require("vue2-waterfall").WaterfallItem;
```
or link as a `script` in an html file and access global variable `Vue2Waterfall`.

```js
<script src="dist/vue2-waterfall.js"></script>
```

## Usage

```html
<Waterfall>
  <WaterfallItem>item1</WaterfallItem>
  <WaterfallItem>item2</WaterfallItem>
  <WaterfallItem>item3</WaterfallItem>
  ...
</Waterfall>
```

## options

### Waterfall Attributes

| Option          | Description                                    | default     | type      | acceptable values        |
| --------------- | ---------------------------------------------- | ----------- | --------- | ------------------------ |
| gutterWidth     | the waterfall brick element horizontal gutter  | 10          | Number    |           -              |
| gutterHeight    | the waterfall brick element vertical gutter    | 10          | Number    |           -              |
| resizable       | triggers layout when browser window is resized | true        | Boolean   |  'true' 'false'          |
| align           | Alignment                                      | 'center'    | String    |  'left' 'center' 'right' |
| fixWidth        | fix the waterfall component width              |      -      | Number    |           -              |
| minCol          | min columns                                    | 1           | Number    |           -              |
| maxCol          | max column                                     |      -      | Number    |           -              |
| percent         | use Fluid layout, ignore waterfallitem width   |      -      | Array     |           -              |

### WaterfallItem Attributes

| Option  | Description                                                 | default     | type      | acceptable values        |
| ------- | ----------------------------------------------------------- | ----------- | --------- | ------------------------ |
| order   | The order of waterfallItem, often be set to index in v-for  |      -      | Number    |           -              |

### Events

| Option         | Description                              |
| -------------- | ---------------------------------------- |
| rendered()     | the waterfall component is rendered      |


## LICENSE

MIT@[PLDaily](https://github.com/PLDaily)
