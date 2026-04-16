# AV Roulette.md

setcpm(120)
_$: s("[hh*16]/1.5,[bd*4]/2.5, [sd*4]/4") .room(0.5) .gain(0.1)
_$: s("[bd*4]/3") .lpf(500) .distort(1) .orbit(100)
_$: s("sd*5/10") .sound("bossdr220_cp") .orbit(100) .delay(".5:1") .room(1) .gain(0.5)
//don't open this one!
_$: s("bd*4") .sound("yamahatg33_bd") .distort(7) .gain(0.05) .lpf(500) .distort(10) .gain(0.05)
//
_$: note("A2, C2, E3") .sound("gm_fx_echoes") .duckorbit(100) .adsr(1,5,2,1) .distort(1) .room(7) .gain(0.2)
_$: n("[A1/4] ~ , ~ E2") .scale("A:min") .sound("gm_synth_bass_1") .adsr(0.5,10,10,10) .lpf(400) .distort(1.5) .crush(16) .room(10) .lpf(130) .gain(0.1)
_$: note("A1") .sound("gm_harpsichord") .tremolosync("4") 
_$: n("[2,8,1]*4/ ~ 1 * 1, ~ 1, [1,2]/ 4") .scale("A:minor") .sound("gm_piano") .lpf(slider(500, 100, 2000, 1)) .room(1)

Thought process:
Working with Isaac's visuals was fun and engaging, he built a live camera visualizer reacting to his movement which allowed me to create fun rhythmic analogies. I started with the drums in the upper part of the code, where I try fun rhythmic ideas that don't usually work by themselves, but layering them with fun effects such as delay, ducking, and drum layering I was able to get textures that speak to me in terms of drums. 

Melodies came naturally, after choosing a sample to play with I was able to create tonal ambiences in the key of A:minor. The piano was a cherry on top with distinct melodies and chord ornaments.


