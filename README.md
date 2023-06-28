# audio-koto-synth-design
My try at emulating a koto

koto is generally A1-A7, tuned to 430Hz. 

# Creating a Koto Synth

I thought it'd be cool to create a Koto-sounding synth in Serum. Here's the process I took

## Harmonics

It appears the koto has all even/odd harmonics.
|Wave|Harmonic series|
|---|---|
|Sine|just fundamental|
|Tri/sq|odd harmonics|
|Saw|Even and odd harmonics|

### Algorithm to find harmonic series
```
F = Fundamental Freq.
H = Harmonic
n = The desired harmonic

Algo:
H = (F*n) 

Say F = 50
Second harmonic = 100Hz = (50*2)
Third harmonic = 150Hz = (50*3)
..etc.
```

## Tuning File
TODO

#### Research
-[ ] I acquired an audio file of a musician playing the Koto and popped that into Ableton to observe the harmonics.
-[ ] I then researched what the tuning was, traditionally, and the notes that comprise the instrument.

#### Serum Edits
-[ ] I set the oscillators to be -40 fine. When observed in the Tuner Audio Effect set to 430, the note was pretty spot on. 
-[ ] I used Pro-Q to observe the harmonics on the synth.
