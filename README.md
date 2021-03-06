# recordselectedwindow
`recordselectedwindow` creates animated gif files by recording windows that are selected with mouse. It is a simple wrapper around `byzanz-record` and it relies on the tools `xdotool` and `xwininfo` for X. 

The default duration for recording is 10 seconds and the default filename for the animation is `WindowRecording{Timestamp}.gif`.

## Usage

To start recording a gif animation with filename `example1.gif`, we write

```
$ ./recordselectedwindow example1.gif
```

The recording starts when we choose a window with the mouse. Since the duration is not specified, the animation in `example1.gif` is a recording of 10 seconds. 

![Example animation 1](example1.gif)

We can change the duration to 5 seconds by 

```
$ ./recordselectedwindow -d 5 example2.gif
```

![Example animation 2](example2.gif)
