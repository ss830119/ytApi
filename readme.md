# YTApi
Demo: 
<a href="https://codepen.io/ss830119/pen/rNaGWZd?editors=0010" target="_blank">https://codepen.io/ss830119/pen/rNaGWZd?editors=0010</a>

## Getting Started
```html
<script src="https://ss830119.github.io/assets/ytapi.js"></script>
```

## Usage

```html
<div id="player"></div>
```
```js
var ytvideo = new YtApi();
ytvideo.addVideo({
    element: 'player',
    name: 'player1',
    videoId: 'SEqfIKQfrg0',
})

// onYouTubeIframeAPIReady is Youtube API
function onYouTubeIframeAPIReady() {
    ytvideo.ytvideo.ready() // init video
}
```

## feature
### addVideo
```js
ytvideo.addVideo({
    element: 'player', // html element
    name: 'player1',  // set videoName
    videoId: 'SEqfIKQfrg0', // Youtube video id
    width: '', // default is '600'
    height: '', // default is '900'
})
```

### playVideo
```js
ytvideo.playVideo(videoName)
```

### stopVideo
```js
ytvideo.stopVideo(videoName)
```