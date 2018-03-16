# vue-hScroller

# Vue hScroller ![version](https://img.shields.io/badge/version-%20v2.2.0%20-green.svg) ![vue](https://img.shields.io/badge/vue-%20v2.1%20-green.svg) 

[Vue Scroller](https://github.com/miracllife/vue-hScroller) is a foundational component of [Vonic](https://github.com/miracllife/vonic) UI.
In purpose of smooth horizontal scrolling, pull to refresh and infinite loading.

> For vue 1.0, please refer to branch v1.

## Demo

[https://miracllife.github.io/vue-hScroller/](https://miracllife.github.io/vue-hScroller/)

## How to use

```bash
npm i vue-hScroller -S
```

```js
/* ignore this if you include vue-hScroller.js by <script> tag from a cdn, such as unpkg */
import Vue from 'vue'
import VuehScroller from 'vue-hScroller'
Vue.use(VuehScroller)
```

```html
<scroller
  :on-refresh="refresh"
  :on-infinite="infinite">
  <!-- content goes here -->
</scroller>
```

[Live Code on JsFiddle](https://jsfiddle.net/miracllife/cpjfr096/)

## Webpack project by vue-cli

https://github.com/miracllife/vue-hscroller-demo

## API

#### Scroller component attributes:

| Attr. Name | Description | Required | Default Value |
|-----|-----|-----|-----|
| onRefresh | pull to refresh callback | N | - |
| onInfinite | infinite loading callback | N | - |
| onInfinite | infinite loading callback | N | - |
| refreshText | tips of `pull-to-refresh` | N | 下拉刷新 |
| noDataText | tips of `no-more-data` when `infinite-loading` finished | N | 没有更多数据 |
| width | scroller container width | N | `100%` |
| height | scroller container height | N | `100%` |
| snapping | enable snapping mode | N | `false` |
| snappingWidth | snapping width | N | 100 (stand for 100px) |
| snappingHeight | snapping height | N | 100 |
| refreshLayerColor | text color of `pull-to-refresh` layer | N | #AAA |
| loadingLayerColor | text color of `infinite-loading` layer | N | #AAA |
| minContentHeight | min content height (px) of `scroll-content` | N | 0 |

#### Scroller vm instance methods:

- `resize()` resize scroller content (**deprecated, cause the scroller's content resizes self automatically**)
- `triggerPullToRefresh()` start pull-to-refresh manually
- `finishPullToRefresh()` stop pull-to-refresh
- `finishInfinite(isNoMoreData :Boolean)` stop infinite-loading
- `scrollTo(x:Integer, y:Integer, animate:Boolean)` scroll to a position in scroller content
- `scrollBy(x:Integer, y:Integer, animate:Boolean)` scroll by a position in scroller content
- `getPosition :Object` get current position of hScroller content



#################################   declaration   ############################################


## For the respect to component coding author, we made this declaration
## This component refferences  the vue-scroller component,whos author named wangdahoo 
## and his lib https://wangdahoo.github.io/vue-scroller
## thanks


################################################################################################
