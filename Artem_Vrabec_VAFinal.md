# Strudel.cc x HYDRA VA Final

THIS IS FOR STRUDEL.CC

setcpm (181)

//VOYD
_$: n("1") .sound("supersaw") 
.distort (5) .lpf(150) .gain(sine.fast(1))
.tremsync(2).tremolodepth("<1 2 .5>")
.adsr(1, 1, 1, 0)
.room("< 1. - 5. >")
.hpf (50)
.gain(0.05)
.adsr(1)

_$: n("1") .sound("supersaw")
.freq (1000) .room(2)
.tremsync(8).tremolodepth("<1 10 .2>")
.gain("<1 0.1 .2>")
.lpf("<100 500 2000>")
.adsr(1)

_$: n("1*16") .sound("supersaw")
.freq (1000) .gain(0.05) 
.vowel ("<a e > <i>") .distort(1)
.room("<1 3 5>")
.adsr(1)

_$: n("1*4/2") .sound("sine")
.freq(40) 
.distort(3) .lpf(40) .resonance(50)
.gain("<0 0.1 0.05 0.005>")
.tremsync(1) .tremolodepth("<7 1 0.5>")
.room(1) .bpf("<10 25 40>")
.adsr(1)

//drums
_$: n("1*16/8") 
.distort(3) .lpf("<50 30 50 100>") 
.freq(50)
.gain("<1 0.1 .2>")

_$: note("100*4") .sound("square")
.tremsync(1) .tremolodepth("<1 0.5 2>")
.gain("<0.05 0.5>") .hpf(1500) .freq(50)
.room(1)

_$: n("1") .sound("supersaw")
.freq(5) 


Documentation: In my Strudel patch I was primarily using basic sounds: Supersaw, Sine, Square with intention to push Strudel beyond the sound capabilites I thought it possesed. For my VA project I wanted to explore use of .freq and sequencing of effect values to see what kind of fun textures and rhythms I can summon. Layering these things was super fun and informative for me as it unlocked a whole new perspective on Strudel. The idea that you can create anything from a single sound source really stands true! 

CODE FOR HYDRA

s0.initVideo('https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOXc0aWFyMWY5eDB6eGlvMmFkeTdveDNidHpvbmhjbHV1MWxqdjA1aiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/In0Lpu4FVivjISX9HT/giphy.mp4')


src(o0)
.modulate(noise(10),0.05)
.blend(shape(4),0.01)
//.color([1, 8], 1)
//.rotate(() => 100)
//.kaleid([10, 2, 60])
.out(o0)

Documentation: 
This is a very simple but effective 

.modulate(noise(10),0.05)
.blend(shape(4),0.01)

this was the main build of the code, it has such lovely warping capabilities it was just so easy to manipulate with simple add ons. Changing the numbers in the code gives such unique deep results! And thank you professor for helping me with the code in class!

Artem
