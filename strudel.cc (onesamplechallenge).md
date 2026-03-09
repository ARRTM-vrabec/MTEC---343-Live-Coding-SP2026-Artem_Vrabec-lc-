setcpm (180/4)


$: n("[20 5 10]/0.5, [12 15 2 10]/4, [1 2 4 6]/4") .scale ("A:Mixolydian") .sound ("gm_acoustic_guitar_nylon")
.room (slider(0.05, .05, 2))  .lpf (slider(200, 200, 15000))
.delay (slider(0.5, 0.5, 1))

$: n("[11 21 1]/0.5, [12 15 2 10]/4 [3 6 9 12]/4") .scale ("A:Mixolydian") .sound ("gm_acoustic_guitar_nylon")
.room (slider(0.05, .05, 2))  .lpf (slider(200, 200, 15000))
.delay (slider(0.5, 0.5, 1)) .gain (0.5)


$: n("[1 2 3 4]/4") .scale ("A:Mixolydian") .sound("gm_acoustic_guitar_nylon")
.gain (slider(0,.0, 5)) .adsr ("1, 1, 1, 0.5") .tremsync(4).tremoloshape("square")
.room (slider(0, .0, 5)) 


$:  n("[0.5*4] [~ ~] [1*4]/4") .scale("A:Mixolydian") .sound ("gm_acoustic_guitar_nylon")
.delay (.5, .10) .lpf (100) .resonance (100)
//.pianoroll() 

$: note("[B1/2] ~ [A1/4]") .scale ("A:Mixolydian") .sound ("gm_acoustic_guitar_nylon")
.distort(5) .lpf (200) .gain (0.1) .adsr (1, 0.5, 1, 2) .room (slider(0.05, .05, 2))
//.tremsync(16).tremoloshape("triangle")

$: n("[7*16]") .sound("gm_acoustic_guitar_nylon")
.bandf(1000) .bandq("<0 1 2 3>") .crush("<16 8 7 6 5 4 3 2>") .gain(1)
