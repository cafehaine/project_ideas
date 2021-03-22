# Remote Game Console

A way to play your game consoles from anywhere in the world.

```
┌──────────┐         ┌────────┐   Capture Card  ┌──────────────────────────┐
│          │  Steam  │        ├─────────────────┤Video                     │
│  Client  ├─────────┤  Host  │                 │           Game Console   │
│          │         │        ├─────────────────┤Controller                │
└──────────┘         └────────┘ Microcontroller └──────────────────────────┘
```

The idea here is to use the Steam infrastructure in order to stream a video
capture from the game console, and send inputs to the console using a
microcontroller wired to a controller.

The microcontroller might need two way communication in order to read the motors
(if Steam supports it).

This will require a program on the host that displays the video capture while
reading the controller inputs and sending them to the microcontroller.

The total BOM would be the following:
- HDMI/RCA capture card ~10€
- Microcontroller ~5€
- Game console (depends)
- Controller (depends)
- Host system (basic x86 system, an old laptop might to the trick) ~50€
