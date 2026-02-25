# What Are the Roles of the HTML Audio and Video Elements, and How Do They Work?
The audio and video elements allow you to add sound and video content to your HTML documents. 

## audio element
The audio element support the popular audio formats:
- mp3
- wav
- ogg
```
<audio src="https://cdn.freecodecamp.org/curriculum/js-music-player/cruising-for-a-musing.mp3" controls loop muted></audio>
```
- src: location of the audio file
- controls: exposes the audio element on the page and allows users to manage audio playback (some browsers like Safari do not display the volume by default when using the controls attribute)
- loop: makes the audio replay continuously
- muted: start the audio in muted state

You can set multiple sources and the browser will pick the first one it understands
```
<audio controls>
  <source src="audio.ogg" type="audio/ogg" />
  <source src="audio.wav" type="audio/wav" />
  <source src="audio.mp3" type="audio/mpeg" />
</audio>
```

## video element
The video element supports the following formats:
- mp4
- ogg
- webm
```
<video
  src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
  loop
  controls
  muted
  width="400"
  poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
></video>
```
- src: location of the audio file
- controls: exposes the audio element on the page and allows users to manage audio playback (some browsers like Safari do not display the volume by default when using the controls attribute)
- loop: makes the audio replay continuously
- muted: start the audio in muted state
- width: set the width of the video player
- poster: display an image while the video is loading

As with the audio, you can set multiple sources and the browser will pick the first one it can play
´´´
<video
  controls
  width="400"
  poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
>
  <source
    src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
    type="video/mp4"
  />
  <source
    src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.webm"
    type="video/webm"
  />
  Your browser does not support the video tag.
</video>
´´´