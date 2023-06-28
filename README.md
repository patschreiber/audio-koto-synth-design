# audio-koto-synth-design
My try at emulating a koto

koto is generally A1-A7, tuned to 430Hz. 

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
