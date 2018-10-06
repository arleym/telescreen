
# Telescreen App

A simple local media player. I like finer speed controls on media. I use this tool to consume or review local media. 

Speed listening and watching is something I've been using more and more over the past two years. I will blog about it and link it up soon on this [arleym.com post](http://arleym.com/experiments-in-reading/). And yep, this app gets it's name from the book 1984 ;) 

If memory serves the way JS is accessing local files for playback wouldn't be ideal security-wise if played over the Internet. This is for `file:///` protocol, not `http*`. 

When speed watching on apps like VLC or Quicktime playback can feel choppy, or are UI is awkward for speed tweaking on the fly, or limiting in max-speed. I've always liked how Blink browsers handle speed controls (I love [Video Speed Control](https://chrome.google.com/webstore/detail/video-speed-controller/nffaoalbilbmmfgbnbgppjihopabppdk) extension, and match keyboard shortcuts). Blink recently removed the 400% audio-playback cap too, making Chrome or Opera ideal tools for speed control.

The code is a bit of a mess, but is a single file with no dependencies. 


## Shortcuts: 

- `space` - pause/play
- `d` - speed up by 10%
- `s` - slow down by 10%
- `r` - reset playback to 100%
- `shift+n` - `n * 100` will be the playback speed
- `esc` - show/hide controls bar
- `left arrow` - back 5 seconds
- `right arrow` - forward 5 seconds


## The future

- Make the `r` shortcut toggle between 100% and the last set speed
- Playlists?
- Make video area a draggable area
- After dragging a video on the `file` input, focus the video
- remember the speed of last played file https://codepen.io/ArleyM/pen/EEmKEa
- start video by URL query string - https://www.sitepoint.com/url-parameters-jquery/ - for Alfred workflow
- JS could use a spring cleaning, cobbled together from tutorials
- Keyboard shortcuts
  - Jump percentages like YT w/ number shortcuts
  - shift arrows to jump 30s
- ? help - panel to list shortcuts
- Dreamy: a query parameter that would set a fade-out time
- Foot pedal pause/play and back 5s for transcription use
