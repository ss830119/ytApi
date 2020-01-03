# YTApi
Demo: 
<a href="https://zxccxz0119.github.io/example/ytapi.html" target="_blank">https://zxccxz0119.github.io/example/ytapi.html</a>

## Getting Started
```html
<script src="https://zxccxz0119.github.io/assets/ytapi.js"></script>
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
    ytvideo.ready() // init video
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

### pauseVideo
```js
ytvideo.pauseVideo(videoName)
```