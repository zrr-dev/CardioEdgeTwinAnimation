Watch Scroll Animation

A concept smartwatch for Moni-Buddy that you drive with your scroll wheel.

Scroll once and the watch wakes up. An ECG trace draws itself. Heart rate locks on. Then a simulated alert fires and the whole chain from sensor to wrist slides into view.

The story, in four scenes
Signal. The AFE4950 records ECG at 500 samples per second. The trace draws across the watch face.
Baseline. Heart rate locks on at 93 BPM with signal quality 97. The ring fills.
Alert. A simulated 128 BPM event turns the ring amber. The watch shakes and pulses.
System. The watch steps aside. Three cards show the path: SK-AM62B board, CardioTwin dashboard, Moni-Buddy backend.
How it works
One pinned stage and one timeline. Your scroll position scrubs the timeline forward and back.
anime.js v4 runs the timeline and the scroll sync.
The ECG line draws with the anime.js SVG drawable helper.
Plain HTML, CSS and JavaScript. No build step. One file.
Built for phones and desktops. It respects reduced-motion settings.
Run it

Open index.html in a browser. It needs internet for the animation library and the fonts.

Part of Moni-Buddy

Team MoniBuddy, HackEdge 2026, Track 1, Edge Digital Twin. The edge side uses a TI AFE4950EVM and a TI SK-AM62B. The board filters the signal and finds heartbeats. The dashboard draws the digital twin.

Honest notes
This is a concept render. The watch is not built.
The 93 BPM value comes from one recorded capture. The 128 BPM alert is simulated.
The ECG shape on the watch is an illustration, not the real signal.
Experimental student prototype. Not a medical device. It does not diagnose.